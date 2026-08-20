---
api_specs:
- filename: tabby-ml-chat-api-openapi.yml
  format: yaml
  label: Tabby Chat API
  slug: tabby-ml-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby-ml/refs/heads/main/openapi/tabby-ml-chat-api-openapi.yml
- filename: tabby-ml-completions-api-openapi.yml
  format: yaml
  label: Tabby Completions API
  slug: tabby-ml-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby-ml/refs/heads/main/openapi/tabby-ml-completions-api-openapi.yml
- filename: tabby-ml-events-api-openapi.yml
  format: yaml
  label: Tabby Events API
  slug: tabby-ml-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby-ml/refs/heads/main/openapi/tabby-ml-events-api-openapi.yml
- filename: tabby-ml-health-api-openapi.yml
  format: yaml
  label: Tabby Health API
  slug: tabby-ml-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby-ml/refs/heads/main/openapi/tabby-ml-health-api-openapi.yml
- filename: tabby-ml-ingestion-api-openapi.yml
  format: yaml
  label: Tabby Ingestion API
  slug: tabby-ml-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby-ml/refs/heads/main/openapi/tabby-ml-ingestion-api-openapi.yml
- filename: tabby-ml-models-api-openapi.yml
  format: yaml
  label: Tabby Models API
  slug: tabby-ml-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby-ml/refs/heads/main/openapi/tabby-ml-models-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tabbyml.com
  spf: true
  spf_record: v=spf1 +include:spf.onlarksuite.com -all
hosts:
- host: www.tabbyml.com
  hsts: true
  hsts_max_age: 31536000
  https: true
- host: tabby.tabbyml.com
  hsts: false
  https: true
kind: domain-security
layout: security
method: probed
name: Tabby Ml Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tabby, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS; 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Tabby
provider_slug: tabby-ml
slug: tabby-ml-domain-security
source_filename: tabby-ml-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + website hosts\nhosts:\n- host: www.tabbyml.com\n  https: true\n  hsts: true\n  hsts_max_age: 31536000\n- host: tabby.tabbyml.com\n  https: true\n  hsts: false\ndomains:\n- domain: tabbyml.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 +include:spf.onlarksuite.com -all\n  dmarc: false\nnotes: >-\n  Probes captured 2026-07-11. The documented Tabby API is self-hosted, so the\n  live API host is your own instance (default http://localhost:8080) rather than\n  a TabbyML-operated domain; these probes cover the marketing site\n  (www.tabbyml.com) and docs (tabby.tabbyml.com) only. Self-hosted TLS/HSTS is a\n  function of how you expose your own deployment.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tabby-ml/refs/heads/main/security/tabby-ml-domain-security.yml
summary_line: HSTS
tags:
- AI Coding Assistant
- Code Completion
- Open-Source
- Developer Tools
- LLM
- Artificial Intelligence
- Self-Hosted
- Code Generation
- Copilot Alternative
---
