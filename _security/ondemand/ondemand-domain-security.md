---
api_specs:
- filename: ondemand-openapi.json
  format: json
  label: OnDemand AI API
  slug: ondemand-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ondemand/refs/heads/main/openapi/ondemand-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: on-demand.io
  spf: true
hosts:
- cert_expires: Sep  6 12:31:38 2026 GMT
  host: docs.on-demand.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 12:55:04 2026 GMT
  host: api.on-demand.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 03:07:26 2026 GMT
  host: gateway-dev.on-demand.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ondemand Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ondemand, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ondemand
provider_slug: ondemand
slug: ondemand-domain-security
source_filename: ondemand-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.on-demand.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 12:31:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.on-demand.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 12:55:04 2026 GMT\n  hsts: null\n- host: gateway-dev.on-demand.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 03:07:26 2026 GMT\n  hsts: null\ndomains:\n- domain: on-demand.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ondemand/refs/heads/main/security/ondemand-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- RAG
- Agents
- LLM
- Platform as a Service
- Chat
- Workflow Automation
- Vector Search
---
