# CSS Specificity Issue with :hover

This repository demonstrates a common issue in CSS involving specificity and the `:hover` pseudo-class.  The inner `div`'s `:hover` style is unintentionally overridden by the outer `div`'s style due to higher specificity.

## Bug Description

The provided CSS code uses nested divs. The outer `div` has a general `:hover` style, while the inner `div` also has a `:hover` style. Due to specificity rules, the outer `div`'s `:hover` style takes precedence, overriding the inner `div`'s intended hover behavior.

## Solution

The solution involves increasing the specificity of the inner `div`'s `:hover` style to override the outer `div`'s style.  This can be achieved using more selectors or using the `!important` flag (although `!important` is generally discouraged for maintainability reasons).