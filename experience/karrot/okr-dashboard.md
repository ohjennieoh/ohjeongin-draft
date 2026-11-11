# OKR Dashboard

### Team's Pain Point
1. The team had set an annual goal but lacked a clear framework for selecting metrics to measure its performance.
2. As a shared touchpoint across services at different growth stages, chat had to accommodate each service team's distinct needs and expectations.

  | Service Stage | Possible Needs |
  |:---:|---|
  | **Seed / A** | Chat features help users communicate more conveniently |
  | **B / C** | Chat contributes to the service team's success metrics, while a positive experience supports user retention |
  | **D** | Chat supports trust and safety |
<p align="center"><em>Table 1. Potential chat needs across service growth stages.</em></p>
  
### Approach & Rationale
<p align="center">
  <img src="okr-dashboard-procedure.png" width="600">
</p>

**Why categorise services by growth stage first?** \
While each service defines success differently (refer to *Table 1*), services at the same growth stage generally share an overarching goal. Therefore, it is more efficient to first categorise services by growth stage, then refine these categories based on service-specific needs when defining key performance metrics.

**What are the roles of "Primary Success Metric", "Potential Drivers", "Supporting Metrics", and "Guardrail Metrics"?**
* **Primary Success Metric**: the key metric already defined by the service team, used to align the goals of the service and chat teams.
* **Potential Drivers**: metrics defined *within* the chat team to measure the effect of key chat features that may influence the primary success metric.
* **Supporting Metrics**: absolute counts that complement rates and provide additional context, as rates alone can lead to misleading conclusions (e.g. an increase in CTR alongside decreases in total impressions and clicks does not necessarily indicate an overall improvement).
* **Guardrail Metrics**: metrics monitored to ensure that efforts to improve the primary success metric do not negatively affect other important aspects of the service.

**Why is documentation necessary?** \
Documentation records the rationale behind each metric, the cohort it covers (with a diagram for clarity), and the SQL query used to extract the data. It serves as a reference for investigating unexpected data patterns and identifying potential issues.
> [!TIP]
> See AI-Assisted Workflow for how this documentation helped improve the team’s data workflow.
