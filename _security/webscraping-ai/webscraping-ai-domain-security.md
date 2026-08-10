---
api_specs:
- filename: webscraping-ai-account-api-openapi.yml
  format: yaml
  label: WebScraping.AI Account API
  slug: webscraping-ai-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webscraping-ai/refs/heads/main/openapi/webscraping-ai-account-api-openapi.yml
- filename: webscraping-ai-ai-api-openapi.yml
  format: yaml
  label: WebScraping.AI AI API
  slug: webscraping-ai-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webscraping-ai/refs/heads/main/openapi/webscraping-ai-ai-api-openapi.yml
- filename: webscraping-ai-html-api-openapi.yml
  format: yaml
  label: WebScraping.AI HTML API
  slug: webscraping-ai-html-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webscraping-ai/refs/heads/main/openapi/webscraping-ai-html-api-openapi.yml
- filename: webscraping-ai-selected-html-api-openapi.yml
  format: yaml
  label: WebScraping.AI Selected HTML API
  slug: webscraping-ai-selected-html-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webscraping-ai/refs/heads/main/openapi/webscraping-ai-selected-html-api-openapi.yml
- filename: webscraping-ai-text-api-openapi.yml
  format: yaml
  label: WebScraping.AI Text API
  slug: webscraping-ai-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webscraping-ai/refs/heads/main/openapi/webscraping-ai-text-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: webscraping.ai
  spf: true
hosts:
- cert_expires: Oct 20 03:29:54 2026 GMT
  host: webscraping.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 03:29:54 2026 GMT
  host: api.webscraping.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Webscraping Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WebScraping.AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: WebScraping.AI
provider_slug: webscraping-ai
slug: webscraping-ai-domain-security
source_filename: webscraping-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: webscraping.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 03:29:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.webscraping.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 03:29:54 2026 GMT\n  hsts: null\ndomains:\n- domain: webscraping.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webscraping-ai/refs/heads/main/security/webscraping-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web Scraping
- Data Extraction
- Proxies
- Artificial Intelligence
- Browser Automation
- Model Context Protocol
- Development
- Public APIs
- ai
- html
- mcp
- llm-tools
- structured-data
- headless-browser
- captcha
---
