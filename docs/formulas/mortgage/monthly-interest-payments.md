---
title: Monthly Interest Payments
description: How to calculate your monthly mortgage interest payment.
---

## Monthly Interest Payments

The amount of interest you pay each month that does not go towards the home principal amount.

### Code

$$
L = \text{Loan Balance} \\
i = \text{Yearly Mortgage Rate} \\
$$

$$
M = \frac{L \times i}{12}
$$

```ts
function mortgageMonthlyInterest(
    loanBalance: number,
    rate: number
) {
    return (
        loanBalance * rate / 12
    );
} 
```
_Language: TypeScript_

