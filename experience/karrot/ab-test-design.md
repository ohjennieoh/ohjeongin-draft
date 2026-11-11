# A/B Test Design

### Team's Pain Point

1. The team wanted to understand whether changing the notification badge would encourage users to check their notifications, but needed to translate this objective into measurable evaluation criteria.
2. Metric selection required balancing relevance to the test objective, data availability, and sensitivity to users with unusually high unread notification counts.

### My Role

Supported A/B test design by discussing the test objective with the PM, identifying candidate metrics, assessing their feasibility using available data, and explaining the rationale behind the proposed evaluation metrics.
  
### Approach & Rationale

1. **Clarify the test objective**: Discuss the intended user behaviour change with the PM and translate it into a measurable question.
2. **Assess metric feasibility**: Identify candidate metrics and check whether the available data can support their calculation. Where the required data was unavailable, explore alternative ways to measure the intended behaviour.
3. **Justify metric selection**: Evaluate how well each metric reflects the test objective and how its interpretation can be affected by the underlying data distribution.
   1. For the notification badge experiment, considered unread notification counts as an indicator of whether users were checking their notifications.
   2. Compared the mean, 75th percentile (p75), and 90th percentile (p90). Proposed p75 to capture changes in the upper portion of the unread notification distribution, reflecting the goal of encouraging users with larger unread backlogs to check their notifications, while limiting the influence of extreme values compared with the mean.

**What did I consider when selecting key metrics?** \
I aimed to select metrics that could capture improvement while ensuring that it doesn't favour the expected outcome of the new feature. The evaluation criteria needed to reflect the intended user benefit, so that engineering resources would be allocated based on evidence rather than a favourable choice of metrics.


### Outcome

* Contributed to the evaluation and launch of a new notification feature by supporting the definition of A/B test metrics.

[< Karrot](README.md) \
[< Main](../../README.md)
