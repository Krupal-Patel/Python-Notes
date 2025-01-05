
```mermaid
flowchart TD
  rect rgb(144,144,144)
  step1[Understand the Business] --> step2[Understand the Stakeholders]
  step2 --> step3[Explore the Data]
  end
  step3 --> step4[Data Wrangling]
  step4 --> step5[Descriptive Statistics]
  step5 <--> step6[Data Wrangling]
  step6 <--> step5
  step6 --> Insights

```
