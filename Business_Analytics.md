
```mermaid
flowchart TD
  subgraph id1[Frame a Business Problem]
  step1[Understand the Business] --> step2[Understand the Stakeholders
  step2 --> step3[Explore the Data]
  end
  subgraph id2[**Exploratory Data Analysis**]
  step2 --> step3
  step3 --> step4[Data Wrangling]
  step4 --> step5[Descriptive Statistics]
  step5 <--> step6[Data Wrangling]
  step6 <--> step5
  end
  step6 --> Insights

```
