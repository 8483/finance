# Valuation

> **The value of any financial product is always the present value of the future cash flows.**

In other words, if in five years the business is projected to produce cash flow of $20 million dollars, how much is that worth today? You can calculate that as:

```
(20,000,000 / ((1 + r) ^ 5))
```

As you can see, the greater the cash flow, the more the present value (PV) goes up. The farther in the future (years is represented by the 5), the less valuable the cash flow is. The higher the r (discount rate), the less valuable the cash flow is. This would mean the cash flow is riskier. **CAPM is how you calculate the discount rate (r).**

As a side note, often times you'll see trick questions that will try to allude that there are sometimes other factors that can change the value of a business other than the present value of the future cash flows.

# Required Rate of Return

This is based on our individual perspectives dependent on:

-   Investment goals
-   Time horizon
-   Available capital
-   Risk tolerance

If you don't know your required rate of return, we can use a **general (default)** one, based on the **Weighted Average Cost of Capital (WACC)**.

# CAPM vs WACC

CAPM is used in WACC

WACC = What a company is expected to return.

CAPM = Relationship between the expected return of an investment vs the market risk. It represents what the equity investor expects the company to return for them.

**If a company has no debt, then WACC = CAPM**

# Weighted Average Cost of Capital (WACC)

Defines the minimums amount a company needs to return.

Useful for:

-   A company to decide if a project is worth investing in.
    -   Ex. If a project reutrns 5%, and the WACC is 8%, the company would be destroying wealth.
-   An investor to discount future cashflows in a DCF analysis, to determine their present value.
    -   Ex. If we expect $1,000,000 in 2 years, the present value is worth $858,929 with a 7.9% WACC i.e. `$1,000,000 / (1.079^2)`. If there are 10,000 shares outstanding, the present value of a share is $85.89. If the current price is $50, then the company is undervalued.

```
WACC = cost of debt + cost of preferred shares + cost of equity
WACC = Wd * Rd * (1 - t) + Wp * Rp + We * De

W = weight
R = cost (required rate of return)
t = tax rate (deductible for debt)
```

Ex. Company XYZ wants to raise $100,000 capital by:

-   Borrowing $30,000 from a bank (debt) at 4% (cost of debt). Let's say the tax rate is 25%.
    -   30% (weight) of the capital.
-   Selling $70,000 equity (ownership). The cost of equity is defined with **Capital Asset Pricing Model (CAPM)**. Let's say it's 10%.
    -   70% (weight) of the capital.
-   There are no preffered shares.

\* preffered shares -If the company enters bankruptcy, preferred stockholders are entitled to be paid from company assets before common stockholders.

```
WACC =
    30% * 4% * (1 - 0.25)
    + 0 preffered shares
    + 70% * 10%

WACC = 7.9%
```

# Capital Asset Pricing Model (CAPM)

It represents what the equity investor expects the company to return for them.

**CAPM is used to estimate a discount rate for cash flows in a DCF calculation (in particular, the cost of equity)**

CAPM tries to represent the inherent riskiness of an investment. A stock that has been more volatile (in price) in the past is likely to be a risker investment in the future, and it should be discounted appropriately (at a higher discount rate).

The general idea behind CAPM is that investors need to be compensated in two ways:

-   Time value of money
-   Risk

```
Required return on equity = Risk free rate + (Market premium) * Beta.

Re = Rf + (Rm - Rf) * B
```

Ex.

```
# Facebook
3% + (10% - 3%) * 1.2 = 10.2%

# Apple
3% + (10% - 3%) * 0.99 = 8.9%
```

CAPM is a model that describes the relationship between risk and expected return, by showing you the required return on equity i.e. discount rate from future cashflows, while looking at:

-   **Risk-free rate of return** `Rf`

    It's the return you could expect if you were to invest your money at no risk. You can make an argument that's not possible, but that's beside the point. The rate used is usually the return on a 10 year treasury bond. Think of the + Rf as saying that the minimum return you're willing to accept on your investment is what you would get if you invested in the least risky asset in the world.

-   **Expected return from the market** `Rm`

    It's the rate of return the market as a whole produces. In the industry, the S&P 500 is the most common metric used to calculate this, but for whatever reason all my professors demanded we use this. (Rm-Rf) is called the market risk premium, so if a problem ever gives you the market risk premium, don't subtract Rf. It's a super common mistake.

-   **Beta of the investment** `B`

    Beta is a correlation between the market and the asset in question. So a Beta of 1 would mean your asset always returns the same as the market. 0 would mean there is no correlation. Higher Beta = more risk (again, there are good arguments as to why this isn't true, but for the purposes of the CAPM that's what it means).

# Discounted Cash Flow (DCF)

DCF is a function for corporate finance and projection of investment within a company/firm which is attempting to embark on a new project. Trying to apply DCF to public market valuation and stock investment doesn't make a whole lot of sense in 2021. Market valuations and stock prices do not adhere to the same set of circumstances and reality that DCF valuations do.

https://youtu.be/V4YAY6zpJ2E

Imagine you are buying a whole business, and you get to keep all the cash it produces each year, called `free cash flow`.

To figure out the value of the business, you model out 10 years of free cash flow you are likely to recieve as the new owner as the business grows/shrinks, and then you are going to sell the business.

In other words:

1. You dump a whole lot of money
2. Get 10 years of FCF.
3. Recieve a big lump of money at the end.

You now need to dicount each of those annual cashflows by the annual return you want to achieve each year ex. 15%, to figure out what all of that is worth today.

Ex. If you predict you are going to get $100 at the 8th year of ownership, you only want to pay $32.70 today because that's the same as investing $32.70 and growing it 15% YoY for 8 years.

You also need to discount the sell price at the 10 year mark.

This gives you the `intrinsic value` of the business. This is the fair value of the business today to achieve 15% each year.

How do you know what each year's FCF is going to be? You don't... You forecast it based on past performance.

The YoY growth rate has the biggest impact on the valuation. This is why some stocks have insane valuations, because investors predict huge growth in the future.

# Reverse engineering DCF

What growth rate would the stock have to show annualy over 10 years to justify buying the shares at the current market cap?

Example:

Tesla despite generating $97B in revenue (April 2025) the past 12 months, has only produced $3.6B in FCF. Assuming you can sell the business after 10 years at x20 FCF multiple, to match the intrinsic value to the current market cap, you'd need a 43% YoY growth.

So, at $480 per share and $1.42T market cap, Tesla would need to show a 52% YoY growth for 10 years. Is this possible?

Tesla grew its REVENUE 42% annualy from 2018 to 2023, but free cash flow is a whole different beast.

Unless the business become wildly more efficient or starts generating substantial high margin cash, both completely dependent on autonomous driving... The valuation is not realistic.

If Tesla achieves the autonomous driving... Then it might be undervalued.
