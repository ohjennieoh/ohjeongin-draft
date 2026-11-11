# AI-Assisted Workflow

### Team's Pain Point
1. The team had no other data analyst, so the PM was responsible for the data workflow. However, without a background in data analysis, the PM lacked confidence in writing SQL queries and structuring query logic.
   1. Difficulty verifying whether query logic accurately reflected intended business assumptions.
   2. Difficulty troubleshooting queries when the results differed from expectations.
2. Without a technical background, it can be difficult to understand what data a SQL query retrieves. Even for those with technical expertise, differences in query-writing styles can make interpreting someone else's queries time-consuming.

### My Role
Designed and refined a Claude Skill to provide the team with AI-assisted SQL review, troubleshooting, and query documentation.
  
### Approach & Rationale

**What key features were incorporated into the Claude Skill?**

* **Explain complex query logic in natural language**: Breaks down CTE dependencies and JOIN logic, including the keys used, into easy-to-understand explanations.
  * Visualises how upstream and downstream CTEs connect and which keys link them, making dependencies and data flow easier to follow.
* **Test edge cases to support troubleshooting**: Uses BigQuery MCP to execute the submitted query and run checks for potential edge cases. Assesses their impact on query results and flags scenarios that could cause issues in future runs.
* **Suggest improvements to query efficiency**: Reviews query logic and recommends changes, prioritised by potential impact and issue severity. Presents proposed edits in a diff format for easy comparison, leaving the final decision on whether to accept each suggestion to the user.

**How was the Skill’s performance evaluated?**

I started with simple queries to verify that the output was formatted and presented as intended. For more complex queries, I independently documented potential edge cases, query logic, and expected CTE relationships, then compared my assessment with Claude’s output. I used any discrepancies to refine the Skill’s instructions and retested it to check whether the changes addressed the errors.

### Outcome

* Improved the efficiency of the team’s data workflow.
  * PMs could revisit previously written queries and understand their purpose and logic, making existing analyses easier to reuse.
* Claude provided preliminary checks and suggestions, helping PMs investigate issues before seeking further assistance.
* Established a more consistent SQL review process through structured checks of query logic, CTE dependencies, and edge cases.
