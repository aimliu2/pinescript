# Volatility
![Volatility](Volatility.png)

# Method
### Kaufman's Efficiency Ratio (KER)
- Compare `avg movement` and `total movement` in l period
- Low vol : Price violently move but end up with little or no movement
- Nominator : Abs.Slope => `|c-c[n]|`
- Denominator : Sum.Abs.delta.price => `sma(abs(c-c[1]),n)`

### Weight Sum ER
- Compare `avg movement` and `total movement` in l period
- Low vol : Price violently move but end up with little or no movement
- Nominator : Abs.Slope => `|c-c[n]|`
- Denominator : Weight Sum.Abs.delta.price => `wma(abs(c-c[1]),n)`

### True Range ER
- Compare `avg movement` and `total movement` in l period
- Low vol : Price violently move but end up with little or no movement
- Nominator : Linear Avg True Range occured in L length=> `TR[L]/L`
- Denominator : ATR => `rma(tr,L)`

# How to read indicator
|Price|Vol|Meaning
|--|--|--|
|unmove|low| Sideway|
|move|low| weak Trend|
|unmove|high| End of swing|
|move|high| Silver Bullet|

# Special
### Stdema
- Compare `avg movement` and `total movement` in span period
- Low vol : Price moved close to ema
- Nominator : Std in L length => `std(l)`
- Denominator : Std in span length => `(std(l),span)`