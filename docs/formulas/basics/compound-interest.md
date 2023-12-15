---
sidebar_position: 1
title: Compound Interest
description: Calculating compound interest
---


# Compound Interest

$$
A = \text{Accrued amount (the future value of the investment/loan)} \\
P = \text{Principal amount (initial investment/loan)} \\
r = \text{Annual interest rate (decimal)} \\
t = \text{Time in years} \\
n = \text{Number of times the interest is compounded per year} \\
$$

$$
A = P \times \left(1 + \frac{r}{n}\right)^{n \times t} \\
$$

## Example

$$
P = \$5000 \\
r = 8\% = 0.08 \\
t = 2 \text{ years} = 2 \\
n = \text{Quarterly} = 4
$$

$$
A = 5000 \times \left(1 + \frac{0.08}{4}\right)^{4 \times 2} \\
A = 5000 \times 1.02^8 \\
A = ~5858.3
$$

## Code

```ts
function compoundInterest(
    principal: number,
    rate: number,
    compoundPeriods: number,
    years: number,
) {
    return (
        principal * Math.pow(
            1 + (rate / compoundPeriods),
            compoundPeriods * years
        )
    );
}
```
