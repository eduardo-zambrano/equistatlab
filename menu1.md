+++
title = "Protected Income and Inequality Aversion"
hascode = true
date = Date(2019, 3, 22)
rss = "A short description of the page which would serve as **blurb** in a `RSS` feed; you can use basic markdown here but the whole description string must be a single line (not a multiline string). Like this one for instance. Keep in mind that styling is minimal in RSS so for instance don't expect maths or fancy styling to work; images should be ok though: ![](https://upload.wikimedia.org/wikipedia/en/3/32/Rick_and_Morty_opening_credits.jpeg)"

tags = ["syntax", "code"]
+++


# Protected Income and Inequality Aversion
The material below is based on work in progress by [Eduardo Zambrano](https://eduardo-zambrano.github.io/ and [Marc Fleurbaey](https://sites.google.com/site/marcfleurbaey/Home).

When evaluators contemplate a policy reform, they must think about the differential effects those policies may have on different individuals. Below we contemplate the evaluation of policy reforms relative to a status quo. If the policy reform generates only winners and no losers relative to the status quo, an evaluator may be strongly inclined to favor the reform over the status quo. Unfortunately, most policy reforms generate both winners and losers, and an evaluator must then determine how to trade off those gains and losses, if a decision must be made.

Let's consider several ways in which those gains and losses may be assessed. For illustrative purposes, we consider situations where a reform affects only two individuals, and leaves the rest of the individuals unaffected. 

In the illustration below, income is used as the index of individual advantage in, but the analysis is relevant to any setting in which individual advantage is measured by a cardinally measurable and interpersonally comparable index. In particular, it is possible to adjust income for non-market aspects of quality of life that individuals enjoy or endure, and use this ajusted income (usually called “equivalent income”) as the relevant index instead of ordinary income.

## Inequality Neutral (IN)
The IN evaluator only cares about the total sum of income associated with a policy, and not with its distribution.

~~~
<iframe src="https://www.desmos.com/calculator/m6lqfgk4kj?embed" width="100%" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>
~~~

## Constant Difference Protected Income (CDPI)
An evaluator with CDPI social preferences would reject policies that, when compared to a status quo of equality, entail one of the individuals losing more than a certain amount of income, $L$, with $L$ being constant for all income levels, $y$, in the status quo.

~~~
<iframe src="https://www.desmos.com/calculator/fctoakmwnd?embed" width="100%" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>
~~~

## Constant Relative Protected Income (CRPI)
An evaluator with CRPI social preferences would reject policies that, when compared to a status quo of equality, entail one of the individuals losing more than a certain fraction of income, $k$, with $k$ being constant for all income levels, $y$, in the status quo.
~~~
<iframe src="https://www.desmos.com/calculator/c0csn0sbia?embed" width="100%" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>
~~~



---