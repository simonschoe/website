---
## Configure page content in wide column
title: |
  <style>
    .typewriter {
      overflow: hidden; /* Ensures the content is not revealed until the animation */
      border-right: .15em solid orange; /* The typewriter cursor */
      white-space: nowrap; /* Keeps the content on a single line */
      letter-spacing: .0em; /* Adjust as needed */
      animation:
        typing 4s steps(24) 1s 1 normal both,
        blink-caret .75s steps(44) infinite normal;
    }

    /* The typing effect */
    @keyframes typing {
      from { width: 0 }
      to { width: 7.8em } /* Manually set to stop after last character */
    }

    /* The typewriter cursor effect */
    @keyframes blink-caret {
      from, to { border-color: transparent }
      50% { border-color: orange }
    }
  </style>

  <h1 class="f2 f1-m f-headline-l fw5-ns mv4 lh-solid tracked-tight-ns typewriter" style="font-family: inherit;">Hi, I’m Simon. 🪄</h1>
number_featured: 2 # pulling from mainSections in config.toml
use_featured: false # if false, use most recent by date
number_categories: 10 # set to zero to exclude
show_intro: true
intro: |
  I am a data scientist at Provinzial where I work on RAG systems and domain-specific AI applications. I am driven by curiosity and approach my work with a [scientific mindset](https://hbr.org/2022/05/act-like-a-scientist). I enjoy deep work and continuously learning new things.
  
  I hold a PhD in Accounting. In my [research](/research), I have broadly focused on measurement problems in accounting. I have applied traditional quantitative methods as well as novel techniques from machine learning, natural language processing, interpretable machine learning, and causal machine learning to evaluate the prediction of accounting estimates, the analysis of corporate narratives, and the estimation of causal effects.
  
  ---

  1. *Data Ingestion & Processing*<br>
  <font size="3.5">
  Web Scraping: [rvest](https://rvest.tidyverse.org/), [Beautiful Soup](https://beautiful-soup-4.readthedocs.io/en/latest/), [Selenium](https://selenium-python.readthedocs.io/)<br>
  Streaming: [Apache Kafka](https://kafka.apache.org/)<br>
  Query Languages: SQL
  </font>
  
  2. *Data Analysis & Visualization*<br>
  <font size="3.5">
  Data Wrangling: [pandas](https://pandas.pydata.org/), [tidyverse](https://www.tidyverse.org/)<br>
  Plotting Libraries: [ggplot2](https://ggplot2.tidyverse.org/)<br>
  Dashboards & Visual Analytics: [Kibana](https://www.elastic.co/kibana)
  </font> 
  
  3. *Machine Learning & Statistical Modeling*<br>
  <font size="3.5">
  Machine Learning: [tidymodels](https://www.tidymodels.org/), [scikit-learn](https://scikit-learn.org/stable/), [DoubleML](https://docs.doubleml.org/stable/index.html)<br>
  Model Interpretability: [DALEX](https://dalex.drwhy.ai/)<br>
  Data Labeling: [prodigy](https://prodi.gy/)
  </font>
  
  4. *Deep Learning & Natural Language Processing*<br>
  <font size="3.5">
  DL Frameworks: [pytorch](https://pytorch.org/), [transformers](https://huggingface.co/docs/transformers/index)<br>
  NLP: [spacy](https://spacy.io/)
  </font>
  
  5. *Experimentation & Prototyping*<br>
  <font size="3.5">
  Experiment Tracking: [Weights & Biases](https://wandb.ai/site)<br>
  Interactive Prototyping: [gradio](https://www.gradio.app/)
  </font> 
  
  6. *Reproducibility & Documentation*<br>
  <font size="3.5">
  Literate Programming: [Jupyter Notebooks](https://jupyter.org/), [R Markdown](https://rmarkdown.rstudio.com/)
  </font>
  
  7. *Software Engineering & APIs*<br>
  <font size="3.5">
  API Development: [FastAPI](https://fastapi.tiangolo.com/)<br>
  Version Control: [Git](https://git-scm.com/)
  </font>
  
  8. *MLOps & Deployment*<br>
  <font size="3.5">
  CI/CD & Orchestration: Kubernetes, ArgoCD
  </font>
  
  9. *Infrastructure & Observability*<br>
  <font size="3.5">
  Monitoring & Logging: Dynatrace, [Kibana](https://www.elastic.co/kibana)<br>
  Search & Analytics Databases: [Elasticsearch](https://www.elastic.co/elasticsearch)<br>
  </font>
  
show_outro: false
outro: 
---

\*\* index doesn't contain a body, just front matter above. See about/list.html in the layouts folder \*\*
