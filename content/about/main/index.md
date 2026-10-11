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

  <h1 class="f2 f1-m f-headline-l fw5-ns mv4 lh-solid tracked-tight-ns typewriter" style="font-family: inherit;" aria-label="Hi, I'm Simon. 🦦"><span class="tw-ghost" aria-hidden="true">Hi, I'm Simon. 🦦</span></h1>

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
  I am a Data Scientist & AI Engineer at Provinzial, where I work on the enterprise GenAI platform, document processing, RAG, MCP infrastructure, and domain-specific AI products. I translate business needs into AI use cases, design end-to-end solutions, carry out compliance assessments, and seek to promote GenAI adoption across the organization.<br><br>
  I am driven by a deep curiosity and approach my work with a [scientific mindset](https://hbr.org/2022/05/act-like-a-scientist). I enjoy hard problems, cross-team collaboration, and constantly learning new things.<br><br>
  I hold a Ph.D. in Accounting from the University of Münster. In my [research](/research), I have focused on measurement problems in accounting. I have designed and taught [courses](/teaching) on machine learning, data literacy, and insurance economics.
  
  ---

  1. *GenAI & Agents*<br>
  <font size="3">
  Agent Frameworks & Protocols: [Pydantic AI](https://ai.pydantic.dev/), [Model Context Protocol](https://modelcontextprotocol.io/)<br>
  AI Evals: [Pydantic Evals](https://ai.pydantic.dev/evals/)<br>
  LLM Platforms: [Microsoft Foundry](https://azure.microsoft.com/en-us/products/ai-foundry), [Amazon Bedrock](https://aws.amazon.com/bedrock/)<br>
  Retrieval & Search: [Elasticsearch](https://www.elastic.co/elasticsearch)
  </font>
  
  2. *Machine Learning & NLP*<br>
  <font size="3">
  Machine / Deep Learning: [scikit-learn](https://scikit-learn.org/), [PyTorch](https://pytorch.org/), [transformers](https://huggingface.co/docs/transformers/index)<br>
  Causal Machine Learning: [DoubleML](https://docs.doubleml.org/stable/index.html)<br>
  NLP & Labeling: [spaCy](https://spacy.io/), [Prodigy](https://prodi.gy/)<br>
  Data Wrangling: [tidyverse](https://www.tidyverse.org/), [pandas](https://pandas.pydata.org/)
  </font>
  
  3. *Backend & Platform*<br>
  <font size="3">
  APIs & Auth: [FastAPI](https://fastapi.tiangolo.com/), [OAuth 2.0](https://oauth.net/2/)<br>
  DevOps: [Docker](https://www.docker.com/), [Kubernetes](https://kubernetes.io/), [Argo CD](https://argo-cd.readthedocs.io/)
  </font>
  
  4. *Streaming & Observability*<br>
  <font size="3">
  Event Streaming: [Apache Kafka](https://kafka.apache.org/)<br>
  Instrumentation: [OpenTelemetry](https://opentelemetry.io/)<br>
  Traces & Logs: [Dynatrace](https://www.dynatrace.com/), [Kibana](https://www.elastic.co/kibana)
  </font>
  
show_outro: false
outro: 
---

\*\* index doesn't contain a body, just front matter above. See about/list.html in the layouts folder \*\*
