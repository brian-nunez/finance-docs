---
title: Monthly Mortgage Payment
description: How to calculate your mortgage payment.
---

# Monthly Mortgage Payment

$$
M = \text{Mortgage Payment} \\
P = \text{Principal amount} \\
i = \text{Monthly mortgage rate} \\
n = \text{Number of months required to repay the loan}
$$

$$
M = \frac{ P \times \left( i \times (1 + i)^n \right) }{ \left( (1 + i)^n \right) - 1 }
$$

The amount you pay each month to buy your home. This calculation does not include the Private Mortgage Insurance (PMI), Homeowners Association (HOA) fees, property taxes, or downpayment.

### Code

```ts
function mortgagePayment(
    principal: number,
    monthlyRate: number, // yearly rate / 12
    loanTerm: number, // in months
) {
    return (
        ( principal * ( monthlyRate * ( Math.pow(1 + monthlyRate, loanTerm) ) ) ) / ( Math.pow( 1 + monthlyRate, loanTerm ) - 1 )
    );
}
```
_Language: TypeScript_
