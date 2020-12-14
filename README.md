# Forex Implied Volatility

An implied volatility is the volatility implied by the market price of an option based on the Black-Scholes option pricing model. A volatility surface is derived from quoted volatilities that provides a way to interpolate an implied volatility at any strike and maturity.

Unlike in other markets that quote volatility versus strike directly, the FX smile is given implicitly as a set of restrictions implied by market instruments and as such a calibration procedure to construct a volatility-delta or volatility-strike smile is used.

The volatility surface in FX market is constructed based on the sticky delta rule. The underlying assumption is that options are valued depending on their delta, so that when the FX spot rate moves and the delta of an option changes accordingly, a different implied volatility has to be used into the option pricing formula.

Therefore, FX volatility smile is represented by three entities: at-the-money (ATM) volatility, risk reversal, and butterfly.

The ATM volatilities quoted by brokers can have various interpretations depending on currency pairs. Here we introduced the most popular one used by the FX brokers. The ATM volatility is the value from the smile curve where the strike is such that the delta of the call equals, in absolute value, that of the put (this strike is called ATM “straddle” or ATM “delta neutral”).

A risk reversal (RR) is a combination of a long call option and a short put option with the same maturity. This is a zero-cost product as one can finance a call option by selling a put option. Risk reversal volatility is the difference between the volatility of the call option and the put option at the same moneyness level, i.e.,

    25 RR = 25 Delta Call Vol – 25 Delta Put Vol

A butterfly (BF) is a combination of a long call option, a long put option, a short ATM call option, and a short ATM put option. Butterfly volatility is the average of the difference between the volatility of the call option and put option minus the ATM volatility, i.e.,

25 BF = (25 Delta Call Vol + 25 Delta Put Vol)/2 - ATM

The volatility surface in FX market is constructed based on the sticky delta rule. The underlying assumption is that options are valued depending on their delta, so that when the FX spot rate moves and the delta of an option changes accordingly, a different implied volatility has to be used into the pricing formula.

You can find more details at
https://finpricing.com/lib/FxVolIntroduction.html

