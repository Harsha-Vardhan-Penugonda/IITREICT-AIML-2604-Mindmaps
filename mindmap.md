```mermaid
%%{init: {'flowchart': {'nodeSpacing': 70, 'rankSpacing': 85, 'diagramPadding': 30}}}%%
flowchart TB
  subgraph foundation[" "]
    direction TB
    M1["<b>Previous Module</b><br/>Module 1: Python Programming Fundamentals<br/><i>(Python, Flow Control)</i><br/>Variables · strings · loops<br/>functions · basic logic"]
    M2["<b>Previous Module</b><br/>Module 2: Data Handling Toolkit<br/><i>(NumPy, Pandas)</i><br/>Arrays · DataFrames<br/>cleaning · filtering · joins"]
  end

  subgraph path[" "]
    direction TB
    M3U["<b>Current Module Until Previous Session</b><br/>Statistical Thinking, Data Preparation<br/>&amp; ML Workflow<br/><i>(Data understanding, Analysis mindset)</i><br/>Learners now move from<br/>handling data to interpreting data"]

    CUR{{"<b>Current Session</b><br/>Descriptive Statistical Analysis<br/><i>Main mental shift</i><br/>Do not just look at raw data.<br/>Summarize it using mean, median,<br/>variance &amp; standard deviation<br/>to understand patterns and spread."}}
  end

  subgraph value[" "]
    direction LR
    CV["<b>Course value</b><br/>Creates the base for<br/>data visualization, EDA,<br/>feature engineering &amp;<br/>machine learning model decisions"]

    RL["<b>Real-life value</b><br/>Example: A business has daily sales data.<br/>Mean shows average sales,<br/>median shows typical sales without outlier impact,<br/>variance and standard deviation show<br/>how stable or unpredictable the sales are.<br/>This helps teams plan stock, offers,<br/>targets and risk better."]
  end

  subgraph future[" "]
    direction TB
    M4["<b>Upcoming Module</b><br/>Module 4: Supervised Learning<br/><i>(Regression, Classification)</i><br/>Predict numbers and categories<br/>using clean, understood data"]
    M5["<b>Upcoming Module</b><br/>Module 5: Advanced ML<br/>&amp; Unsupervised Learning<br/><i>(Validation, Clustering)</i><br/>Improve models and<br/>discover hidden groups"]
    M6["<b>Upcoming Module</b><br/>Module 6: Advanced GenAI Concepts<br/><i>(LLMs, RAG)</i><br/>Use data understanding<br/>inside GenAI applications"]
  end

  M1 ==>|&nbsp;Foundation&nbsp;| M2
  M2 ==>|&nbsp;Data skills&nbsp;| M3U
  M3U ==>|&nbsp;Analysis mindset&nbsp;| CUR
  CUR ==>|&nbsp;Course path&nbsp;| CV
  CUR ==>|&nbsp;Real-life use&nbsp;| RL
  CUR ==>|&nbsp;Next module&nbsp;| M4
  M4 ==>|&nbsp;Next module&nbsp;| M5
  M5 ==>|&nbsp;Next module&nbsp;| M6

  classDef prev fill:#e3f2fd,stroke:#1565c0,color:#0d47a1
  classDef currMod fill:#fffde7,stroke:#f9a825,color:#5d4037
  classDef currSes fill:#fff3e0,stroke:#e65100,color:#3e2723,stroke-width:5px
  classDef val fill:#e8f5e9,stroke:#2e7d32,color:#1b5e20
  classDef fut fill:#fce4ec,stroke:#ad1457,color:#880e4f

  class M1,M2 prev
  class M3U currMod
  class CUR currSes
  class CV,RL val
  class M4,M5,M6 fut

  linkStyle default stroke-width:3px
```
