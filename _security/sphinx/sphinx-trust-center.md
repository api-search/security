---
certifications:
- SOC 2 Type 2
description: Sphinx maintains a trust center at trust.sphinx.ai (live, HTTP 200). The homepage at sphinx.ai states the product is "SOC 2 Type 2 compliant with zero data retention." The trust-center page is a client-rendered app whose certification list did not render to the fetcher, so the SOC 2 Type 2 claim is captured from the marketing homepage as the verifiable evidence; deeper cert detail would require the rendered trust portal.
kind: trust-center
layout: security
name: Sphinx Trust Center
name_suffix: Trust Center
overview: Sphinx maintains a public trust center documenting SOC 2 Type 2 compliance.
provider_name: Sphinx
provider_slug: sphinx
slug: sphinx-trust-center
source_filename: sphinx-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nprobe: false\nsource: https://trust.sphinx.ai\nurl: https://trust.sphinx.ai\ndescription: >-\n  Sphinx maintains a trust center at trust.sphinx.ai (live, HTTP 200). The\n  homepage at sphinx.ai states the product is \"SOC 2 Type 2 compliant with zero\n  data retention.\" The trust-center page is a client-rendered app whose\n  certification list did not render to the fetcher, so the SOC 2 Type 2 claim is\n  captured from the marketing homepage as the verifiable evidence; deeper cert\n  detail would require the rendered trust portal.\ncertifications:\n  - {name: SOC 2 Type 2, source: https://sphinx.ai}\ndata_posture:\n  zero_data_retention: true\n  note: >-\n    Code execution happens on the user's own kernel; Sphinx advertises a zero\n    data retention posture for customer data.\ndocs:\n  - https://trust.sphinx.ai\n  - https://sphinx.ai\nevidence:\n  - {source: https://trust.sphinx.ai, status: 200, keywords: [trust center]}\n  - {source:\
  \ https://sphinx.ai, keywords: [soc 2 type 2, zero data retention]}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sphinx/refs/heads/main/security/sphinx-trust-center.yml
summary_line: SOC 2 Type 2
tags:
- Company
- Artificial Intelligence
- Data Science
- Data Governance
- Analytics
- AI Agents
- Developer Tools
- Jupyter
- LLM
- Data Reliability
trust_url: https://trust.sphinx.ai
---
