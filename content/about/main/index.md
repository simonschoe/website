---
## Configure page content in wide column
title: |
  <style>
    .typewriter { position: relative; }
    .typewriter.tw-on .tw-ghost { visibility: hidden; }
    .tw-typed { position: absolute; inset: 0; }
    .tw-typed::after {
      content: "";
      display: inline-block;
      width: .06em;
      height: .85em;
      margin-left: .06em;
      vertical-align: -.04em;
      background: orange;
      transition: opacity .6s ease;
    }
    .tw-typed.tw-done::after { animation: tw-blink 1s steps(1) 3; }
    .tw-typed.tw-gone::after { opacity: 0; }
    @keyframes tw-blink { 50% { opacity: 0; } }
  </style>

  <h1 class="f2 f1-m f-headline-l fw5-ns mv4 lh-solid tracked-tight-ns typewriter" style="font-family: inherit;" aria-label="Hi, I’m Simon. 🪄"><span class="tw-ghost" aria-hidden="true">Hi, I’m Simon. 🪄</span></h1>

  <script>
    (function () {
      var h = document.querySelector(".typewriter");
      if (!h || window.matchMedia("(prefers-reduced-motion: reduce)").matches) return;
      var chars = Array.from(h.textContent); // keeps the emoji in one piece
      var out = document.createElement("span");
      out.className = "tw-typed";
      out.setAttribute("aria-hidden", "true");
      h.appendChild(out);
      h.classList.add("tw-on");
      var i = 0;
      function next() {
        if (i === chars.length) {
          out.classList.add("tw-done");
          setTimeout(function () { out.classList.add("tw-gone"); }, 3000);
          return;
        }
        var c = chars[i++];
        out.textContent += c;
        // human rhythm: slight jitter, a beat after punctuation
        var delay = 55 + Math.random() * 45;
        if (c === "," || c === ".") delay += 280;
        setTimeout(next, delay);
      }
      setTimeout(next, 500);
    })();
  </script>
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
