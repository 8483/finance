Options are derivatives. They expire every 3rd Friday of each month.

## Types

CALL - Right to buy at strike price within date. Makes money from price increase.

PUT - Right to sell at strike price within date. Makes money from price decrease.

## Actions

BUY = ASK (lowest price someone is willing to sell)

SELL = BID (highest price someone is willing to buy)

Buy

-   Buy Call options
-   Sell Call options
-   Buy Put options
-   Sell Put options

# Example

Emily owns 100 Verizon shares, bought at $57, the current price is $60. She wants to sell, but doesn't mind holding.

Jimmy likes the stock and thinks it will go up, but can't buy 100 shares.

So, Emily decides to sell 1 CALL option, and Jimmy to buy it. Jimmy is buying the right to buy the 100 shares at a certain price, by a certain date.

## Options chain

Last price: $60  
Expiration: March 20, 2020 (in 71 days)

| Bid   | Ask   | Strike Price |
| ----- | ----- | ------------ |
| $5.00 | $5.10 | $55.00       |
| $2.95 | $2.99 | $57.50       |
| $1.39 | $1.42 | $60.00       |
| $0.48 | $0.49 | $62.50       |
| $0.12 | $0.13 | $65.00       |

Expiration: April 17, 2020 (in 100 days)

| Bid   | Ask   | Strike Price |
| ----- | ----- | ------------ |
| $5.05 | $5.20 | $55.00       |
| $3.10 | $3.15 | $57.50       |
| $1.56 | $1.58 | $60.00       |
| $0.59 | $0.60 | $62.50       |
| $0.16 | $0.18 | $65.00       |

Emily `SELL`s a `apr17'21 62.5 CALL` option. She is immediately deposited the $59 premium (100 shares x $0.59)

Emily bought the shares @ $57 so she is fine selling them at $62.5

Jimmy `BUY`s a `apr17'21 62.5 CALL` option. He is immediately deducted the $60 premium (100 shares x $0.60)

What happens now is they both wait. Jimmy owns the option, and can choose to exercise it i.e. give Emily $6,250 for the 100 shares. Emily still owns the shares.

If Emily didn't own the shares, it would be called an uncovered/naked option.

## Scenario 1 - $61 at expiration

The options expires worthless because Jimmy can buy the stock at the current $61 price, instead of the higher CALL option at $62.5.

Jimmy loses the $60 premium, while Emily keeps her shares, and the $59 from selling the option.

Emily can do this indefinitely, unitl the shares get CALLed away from her.

## Scenario 2 - $65 at expiration

The option Jimmy bought at $0.60 currently trades at $2.50.

Jimmy can now either exercise the option i.e get the 100 shares for $6,250 or sell the option (99% of the cases), where he'd get:

```
100 x $2.50 = 250
```

for a profit of

```
100 x $2.50 - 100 x $0.60
= $250 - $60
= $190

return of 316%
```

The same as

```
100 x $60 - 100 x $62.50
= $6,000 - $6,250
= $250

return of 4%
```

Emily can keep her shares by BUYing the same day $2.50 CALL option, for a $190 loss.

# Greeks

## Delta

Change in stock price to option price

```

DELTA: 0.3
price: $13.85 option: $3.30 + $1 + $0.30
price: $14.85 option: $3.60

```

The close the current price gets to the strike price, the higher the delta gets. The more in the money the option is, the closer to 100% the delta gets.

Calls have positive delta, whereas puts have negative delta.

## Gamma

Gamma is a subset of delta, measuring the rate of which delta changes over time.

The further in our out of the money the option goes, the lower gamma gets, meaning that gamme is highest at the strike price.

## Theta

Price sensitivity to time decay.

Theta is a negative number, as time always flows forward.

## Vega

Price sensitivity to volatility.

Buy options at low volatility, sell at high volatility.

## Rho
