Statistical Tables
==================

R may be used to get all statistical tables information.

Each probability distribution is named (t, f, chisq). By preceeding these names with letters you can ask for various results that are based on this probability distribution.

* **d** density (heigth of ordinate, y)
* **p** probability (probability, CDF, Cumulative Distribution Function, area below curve)
* **q** quantile (x values e.g. for a quantile, sig. level, x-coordinate)
* **r** random (for generation of random values of certain distribution) 

Some examples

```R
# F-krit für Zähler-df=100, Nenner-df=10 Freiheitsgrade bei Alpha = 0.05
qf(0.05, 100, 10, lower.tail = FALSE)

# t-krit für df=22 Freiheitsgrade bei Alpha = 0.05 einseitig
qt(0.05, 22, lower.tail = FALSE)

# t-krit für df=55 Freiheitsgrade bei Alpha = 0.01 zweiseitig
# Achtung, für zweiseitige Fragestellung wird der Alpha-Wert halbiert
qt(0.005, 55, lower.tail = FALSE)

# Chi-Quadrat für df=100 Freiheitsgrade bei Alpha = 0.01
qchisq(0.01, 100)

# Binomialverteilung
# Wahrscheinlichkeit, bei 3 mal Münzwurf zwei mal Zahl zu bekommen 
# n=3, k=2, p=0.5
dbinom(2, 3, 0.5)

# Standardnormalverteilung
# z-Wert der die unteren 2.5% der Fläche unter der Verteilung abschließt
qnorm(.025, 0, 1, lower.tail=T)

# z-Transformation von IQ-Werten
# iq = 95, MW=100, sd=15
# z = (x - MW)/sd
# welchen Prozentrang hat dieser Proband?
z <- (95 - 100)/15
pnorm(z, 0, 1)  # Proband hat Prozentrang von 37, also 37% der Pop sind weniger intelligent als er

# Erzeugen einer normalverteilten Gruppe von 1000 IQs
iqs <- rnorm(1000, 100, 15)
# und zur Kontrolle ansehen
hist(iqs)
qqnorm(iqs)
qqline(iqs)
```


List of distributions available:

Distribution | R name | additional arguments
:--- | :--- | :---
beta | beta | shape1, shape2, ncp
binomial | binom | size, prob
Cauchy | cauchy | location, scale
chi-squared | chisq | df, ncp
exponential  | exp  | rate
F  | f  | df1, df2, ncp
gamma  | gamma  | shape, scale
geometric  | geom  | prob
hypergeometric  | hyper  | m, n, k
log-normal  | lnorm  | meanlog, sdlog
logistic  | logis  | location, scale
negative  | binomial  | nbinom size, prob
normal  | norm  | mean, sd
Poisson  | pois  | lambda
Student's t  | t  | df, ncp
uniform  | unif  | min, max
Weibull  | weibull  | shape, scale
Wilcoxon  | wilcox  | m, n