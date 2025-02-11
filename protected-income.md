+++
title = "Protected Income and Inequality Aversion"
hascode = true
date = Date(2024, 4, 18)
rss = "We develop a methodology for determining an evaluator's social preferences based on the tradeoffs between the well-being of different individuals that the evaluator considers acceptable."

tags = ["syntax", "code"]
+++


# Project 1: Protected Income and Inequality Aversion
The material below is based on the paper [Protected Income and Inequality Aversion](https://osf.io/tnu2q/), by [Marc Fleurbaey](https://sites.google.com/site/marcfleurbaey/Home) and [Eduardo Zambrano](https://eduardo-zambrano.github.io/).

## Introduction
When evaluators contemplate a policy reform, they must think about the differential effects those policies may have on different individuals. Below we contemplate the evaluation of policy reforms relative to a *status quo*. If a policy reform generates only winners and no losers relative to the status quo, an evaluator may be strongly inclined to favor the reform. Unfortunately, most policy reforms generate both winners and losers, and an evaluator must then determine how to trade off any income gains and losses that the reform generates. In our research, we consider several ways in which those gains and losses may be assessed and compared. 

Here, income is used as the index of individual well-being, but the analysis is relevant to any setting in which individual well-being is measured by a cardinally measurable and interpersonally comparable index. In particular, it is possible to adjust income for non-market aspects of quality of life that individuals enjoy or endure, and use this ajusted income (usually called “equivalent income”) as the relevant index instead of ordinary income.

For illustrative purposes, we consider below situations where a reform affects only two individuals, starting from a position where they have the same income, and leaves the rest of the individuals in society unaffected. 

## Inequality Neutral Evaluations
An *inequality neutral* (*IN*) evaluator only cares about the total sum of income associated with a policy, and not with its distribution. Any such evaluator, however, would accept a policy that generates a large enough gain for one individual even if it means sacrificing all the income of the other individual. Figure 1 below illustrates. The orange line depicts the combinations of income for both individuals that leave the evaluator indifferent. Notice that the orange line hits the axes of the graph, meaning that if a policy generates a large enough income for one of the individuals, the evaluator will accept the policy even if it comes at the expense of the totality of the income of the other individual. This is so when, for example, the status quo is the income profile $(150,150)$, and the policy reform produces instead the income profile $(0,600)$, which corresponds to the purple dot in Figure 1.   

~~~
<div>
    <h3>Figure 1</h3>
<iframe src="https://www.desmos.com/calculator/g4hf7euvtj?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0 title="Figure 1: The *IN* evaluator "></iframe>
</div>
~~~

Evaluators finding this type of income sacrifice unacceptable would accept policies that reduce inequality even if they lead to smaller total income. These evaluators are know as *inequality averse*. Below we describe two possible ways in which evaluators may operationalize their inequality aversion.

## Constant Difference Protected Income Evaluations
An evaluator with social preferences characterized by *constant difference protected income* (*CDPI*) would reject policies that, when compared to a status quo of equality, entail one of the individuals losing more than a certain amount of income, $L$, with $L$ being constant for all income levels, $y$, in the status quo, and $y>L$. Figure 2 below illustrates. The black dot corresponds to the income profile $(500,500)$ and denotes the status quo. The solid green line depicts the combinations of income for both individuals that leave the evaluator indifferent. Notice that the green line does not hits the axes of the graph, meaning that if a policy generates a loss larger than $L=300$ for one of the individuals, the evaluator will reject the policy no matter how large the gain is for the other individual. The green dashed lines show that, as the income of one of the individuals grows without bound, the income for the other individual stays above $y-L = 200$. In the figure, the length of the red horizontal segment denotes the maximal acceptable loss, $L=300$.

To understand these social preferences in some more depth, the reader may want to increase $L$ by 'dragging' the green dot towards the origin, which flattens the green line and makes the evaluator less inequality averse. Dragging the green dot towards the black dot, that is, towards the point $(y,y)$, makes $L$ smaller, and therefore makes the evaluator more inequality averse.

~~~
<div>
    <h3>Figure 2</h3>
<iframe src="https://www.desmos.com/calculator/ibznckd7fj?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0 title="Figure 2: The *CDPI* evaluator"></iframe>
</div>
~~~

An evaluator with *CDPI* preferences, however, would be willing to sacrifice the income of one of the individuals if the starting income of the individuals was smaller than $L$. The readers can verify this for themselves by dragging the green dot in the graph back to $(200,200)$ (so that $L=300$) and then dragging the black dot to, say $(150,150)$. For such income levels of both individuals in the status quo, a policy that leads to the income profile $(0,600)$ would be chosen by the evaluator, even if it has zero income for one of the individuals. 

This essentially says that the *CDPI* social preferences do not embed enough inequality aversion, especially for the poorest individuals in society. It would be desirable for the maximal acceptable loss to be smaller, the smaller the income of the individual is to begin with. To social preferences with that property we turn our attention to below.

## Constant Relative Protected Income Evaluations
An evaluator with social preferences characterized by *constant relative protected income* (*CRPI*) would reject policies that, when compared to a status quo of equality, entail one of the individuals losing more than a certain fraction of income, $l$, with $l$ being constant for all income levels, $y$, in the status quo.

Figure 3 below illustrates. The black dot denotes the status quo and the blue line depicts the combinations of income for both individuals that leave the evaluator indifferent. Notice that the blue line does not hits the axes of the graph, meaning that if a policy generates a loss larger than $l \cdot y$ for one of the individuals, the evaluator will reject the policy no matter how large the gain is for the other individual. The blue dashed lines show that, as the income of one of the individuals grows without bound, the income for the other individual stays above $l \cdot y$. In the figure, the length of the purple horizontal segment denotes the maximal acceptable loss, $l \cdot y$.

To understand these social preferences at some more depth, the reader may want to increase $y$ by dragging the black dot away from the origin, which flattens the blue line and makes the evaluator less inequality averse. Dragging the black dot towards the origin makes $l \cdot y$ smaller, and therefore makes the evaluator more inequality averse. Similarly, the reader may increase $l$ by dragging the blue dot away from the origin, which flattens the blue line and makes the evaluator less inequality averse. Dragging the blue dot towards the black dot, that is, towards the point $(y,y)$, makes $l \cdot y$ smaller, and therefore makes the evaluator more inequality averse. Notice that, unlike the previous two social preferences, no matter how one drags the black or blue dots, the blue curve never crosses the axes of the graph. This evaluator will therefore never allow the income of one of the individuals go to zero even if the income of the other individual grows without bound.

~~~
<div>
    <h3>Figure 3</h3>
<iframe src="https://www.desmos.com/calculator/kwwwax4bou?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0 title="Figure 3: The *CRPI* evaluator"></iframe>
</div>
~~~

## Technical
It is important to be very deliberate about what is it that is being compared across individuals. In the preceeding sections income was used as the index of individual well-being, but the analysis is relevant to any setting in which individual well-being is measured by a cardinally measurable and interpersonally comparable index. In particular, it is possible to adjust income for non-market aspects of quality of life that individuals enjoy or endure, and use this ajusted income, usually called [“equivalent income”](https://academic.oup.com/book/37245/chapter/330083193) or “money-metric utility,” as the relevant index instead of ordinary income. Below we adopt this point of view and consider evaluators with preferences over profiles of equivalent incomes.

All the evaluators we consider rank equivalent income profiles according to social preferences that admit an additively separable [Social Welfare](https://en.wikipedia.org/wiki/Social_welfare_function) representation, that is, the *social welfare* of the equivalent income profile $(y_1,...,y_n)$ in a society with $n$ individuals is given by $W(y_1,...,y_n)=f(y_1)+...+f(y_n)$ for some continuous and strictly increasing function $f$, called the *generator* of $W$. 

The choice of generator determines the kind of evaluator we are facing. In particular:

* The *IN* evaluator is associated with the linear ([*utilitarian*](https://en.wikipedia.org/wiki/Utilitarianism)) generator $f(y)=y.$

* All *inequality averse* evaluators (*IA*) are associated with strictly concave ([*prioritarian*](https://www.cambridge.org/core/books/prioritarianism-in-practice/introduction/22CF2479EE6187C11314621EA1AE1B54))  generators. In particular,
  - The *CDPI* evaluator is the prioritarian evaluator associated with the generator $f(y)=-2^{-\frac{y}{L}}$ for $L>0$.
  - The *CRPI* evaluator is the prioritarian evaluator associated with the  generator $f(y)= - y^{\frac{1}{\log_2 (k)}}$  for $k\in(0,1)$.

These two representations correspond to interpretable formulations of (1) translation-invariant [^1] social preferences and (2) a specific subclass of scale-invariant (homogeneous) [^2] social preferences, respectively. 

We mentioned above that none of the translation-invariant evaluators would offer income protection to individuals whose income was less than $L$. Past that income level, they protect a fraction of income given by $1 - \frac{L}{y}$. Notice that this fraction is smaller, the smaller the income level, $y$, in the status quo. On the other hand, the scale-invariant evaluators considered above protect a constant fraction of income, $k$.

Motivated by these findings, we propose a novel class of social preferences
that, starting from a guaranteed income, protect a higher fraction of the sacrificed individual's income the lower their income. In addition to relating levels of protected income to coefficients of inequality, we also characterize the classes of additively separable social welfare functions that guarantee specific (absolute or relative) levels of protection. See [Fleurbaey and Zambrano 2024](https://arxiv.org/abs/2408.04814) for details.

## Endnotes

[^1]: Known as [the *Kolm-Pollak*](https://www.jstor.org/stable/2527392?seq=1) social preferences. 

[^2]: Known as [the *Kolm-Atkinson*](https://en.wikipedia.org/wiki/Atkinson_index) social preferences.



---