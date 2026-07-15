---
layout: archive
title: "Software"
permalink: /software/
author_profile: true
---

{% include base_path %}

<p>In my day-to-day work, I write a lot of code, especially for privacy-preserving deep learning applications, federated learning, GenAI and LLMs, and privacy-enhancing technologies. In this section, you'll find some of the software I've developed that is openly available.</p>

<h2 style="margin-top: 2rem; margin-bottom: 0.75rem; padding-bottom: 0.35rem; border-bottom: 2px solid #2f4f4f; letter-spacing: 0.01em;">Federated learning, implementation, training, and LLMs</h2>

<div style="margin-bottom: 1rem; padding: 1rem 1.15rem; border: 1px solid #d9e2e8; border-radius: 8px; background: #f8fbfd; box-shadow: 0 1px 2px rgba(0,0,0,0.04);">
  <p><strong><a href="https://github.com/ai4os/ai4os-federated-server">AI4OS Federated Learning Server</a></strong><br>
  Federated Learning server deployed in the AI4EOSC platform, developed using Flower. It integrates: client authentication, differential privacy, metric privacy, carbon footprint monitoring, and divergence detection.</p>
  <p><strong>GitHub repository:</strong> <a href="https://github.com/ai4os/ai4os-federated-server">https://github.com/ai4os/ai4os-federated-server</a></p>
  <p><strong>AI4OS documentation:</strong> <a href="https://docs.ai4eosc.eu/en/latest/howtos/train/federated-flower.html">https://docs.ai4eosc.eu/en/latest/howtos/train/federated-flower.html</a></p>
</div>

<div style="margin-bottom: 1rem; padding: 1rem 1.15rem; border: 1px solid #d9e2e8; border-radius: 8px; background: #f8fbfd; box-shadow: 0 1px 2px rgba(0,0,0,0.04);">
  <p><strong><a href="https://github.com/ai4os/ai4-flwr">AI4EOSC - Flower extensions</a></strong><br>
  AI4EOSC extensions to the Flower library used in the AI4OS FL server.</p>
  <p><strong>GitHub repository:</strong> <a href="https://github.com/ai4os/ai4-flwr">https://github.com/ai4os/ai4-flwr</a></p>
</div>

<div style="margin-bottom: 1rem; padding: 1rem 1.15rem; border: 1px solid #d9e2e8; border-radius: 8px; background: #f8fbfd; box-shadow: 0 1px 2px rgba(0,0,0,0.04);">
  <p><strong>Federated LLMs</strong><br>
  Examples of LLM fine-tuning process in a federated way.</p>
  <p><strong>GitHub repository (1):</strong> <a href="https://github.com/IFCA-Advanced-Computing/federated_llm">https://github.com/IFCA-Advanced-Computing/federated_llm</a></p>
  <p><strong>GitHub repository (2):</strong> <a href="https://github.com/judithspd/ai4os-fedllm-medical">https://github.com/judithspd/ai4os-fedllm-medical</a></p>
  <p><strong>GitHub repository (3):</strong> <a href="https://github.com/judithspd/ai4os-fedllm-medical-v2">https://github.com/judithspd/ai4os-fedllm-medical-v2</a></p>
  <p><strong>Model published in Hugging Face:</strong> <a href="https://huggingface.co/ifca-advanced-computing/Mistral-7B-Instruct-v0.3-EOSC">https://huggingface.co/ifca-advanced-computing/Mistral-7B-Instruct-v0.3-EOSC</a></p>
</div>

<h2 style="margin-top: 2rem; margin-bottom: 0.75rem; padding-bottom: 0.35rem; border-bottom: 2px solid #2f4f4f; letter-spacing: 0.01em;">Privacy toolbox</h2>

<p>More information is available <a href="https://ifca-privacy-toolbox.github.io">here</a>.</p>

<div style="margin-bottom: 1rem; padding: 1rem 1.15rem; border: 1px solid #d9e2e8; border-radius: 8px; background: #f8fbfd; box-shadow: 0 1px 2px rgba(0,0,0,0.04);">
  <p><strong><a href="https://github.com/IFCA-Advanced-Computing/trasgodp">trasgoDP</a></strong><br>
  A Python library that implements a set of mechanisms for Local Differential Privacy (LDP) for numerical and categorical records, and metric privacy for location-based ones. It is particularly well-suited for generating synthetic versions of a dataset using mechanisms that ensure differential privacy.</p>
  <p><strong>Documentation:</strong> <a href="https://trasgodp.readthedocs.io/">Read the Docs</a> | <a href="https://pypi.org/project/trasgodp/">PyPI</a></p>
</div>

<div style="margin-bottom: 1rem; padding: 1rem 1.15rem; border: 1px solid #d9e2e8; border-radius: 8px; background: #f8fbfd; box-shadow: 0 1px 2px rgba(0,0,0,0.04);">
  <p><strong><a href="https://github.com/IFCA-Advanced-Computing/anjana">anjana</a></strong><br>
  A Python library to anonymize sensitive tabular data.</p>
  <p><strong>Documentation:</strong> <a href="https://anjana.readthedocs.io/">Read the Docs</a> | <a href="https://pypi.org/project/anjana/">PyPI</a></p>
  <p>More information can be found in this <a href="https://www.nature.com/articles/s41597-024-04019-z">paper</a>.</p>
  <p>If you are using <em>anjana</em>, you can cite it as follows:</p>

  <div style="margin-top: 0.5rem; padding: 0.85rem 1rem; border: 1px solid #cfd9e2; border-radius: 6px; background: #0f172a; color: #f8fafc; overflow-x: auto;">
  <pre style="margin: 0; white-space: pre-wrap; word-break: break-word;"><code>@article{sainzpardo2024anjana,
  title={An Open Source Python Library for Anonymizing Sensitive Data},
  author={S{\'a}inz-Pardo D{\'\i}az, Judith and L{\'o}pez Garc{\'i}a, {\'A}lvaro},
  journal={Scientific data},
  volume={11},
  number={1},
  pages={1289},
  year={2024},
  publisher={Nature Publishing Group UK London}
}</code></pre>
  </div>
</div>

<div style="margin-bottom: 1rem; padding: 1rem 1.15rem; border: 1px solid #d9e2e8; border-radius: 8px; background: #f8fbfd; box-shadow: 0 1px 2px rgba(0,0,0,0.04);">
  <p><strong><a href="https://github.com/IFCA-Advanced-Computing/pycanon">pyCANON</a></strong><br>
  A Python library to check the level of anonymity of a dataset.</p>
  <p><em>pyCANON</em> is a Python library and CLI to assess the values of the parameters associated with the most common privacy-preserving techniques.</p>
  <p><strong>Documentation:</strong> <a href="https://pycanon.readthedocs.io/">Read the Docs</a> | <a href="https://pypi.org/project/pycanon/">PyPI</a></p>
  <p>More information can be found in this <a href="https://www.nature.com/articles/s41597-022-01894-2">paper</a>.</p>
  <p>If you are using <em>pyCANON</em>, you can cite it as follows:</p>

  <div style="margin-top: 0.5rem; padding: 0.85rem 1rem; border: 1px solid #cfd9e2; border-radius: 6px; background: #0f172a; color: #f8fafc; overflow-x: auto;">
  <pre style="margin: 0; white-space: pre-wrap; word-break: break-word;"><code>@article{sainzpardo2022pycanon,
  title={A Python library to check the level of anonymity of a dataset},
  author={S{\'a}inz-Pardo D{\'\i}az, Judith and L{\'o}pez Garc{\'i}a, {\'A}lvaro},
  journal={Scientific Data},
  volume={9},
  number={1},
  pages={785},
  year={2022},
  publisher={Nature Publishing Group UK London}}
</code></pre>
  </div>
</div>
