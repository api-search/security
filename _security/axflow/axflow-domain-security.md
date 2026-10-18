---
api_specs:
- filename: axflow-chat-api-openapi.yml
  format: yaml
  label: Axflow Chat API
  slug: axflow-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axflow/refs/heads/main/openapi/axflow-chat-api-openapi.yml
- filename: axflow-openai-api-openapi.yml
  format: yaml
  label: Axflow Openai API
  slug: axflow-openai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axflow/refs/heads/main/openapi/axflow-openai-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: axflow.dev
  spf: true
hosts:
- cert_expires: Nov 22 04:37:51 2026 GMT
  host: axflow.dev
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Axflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axflow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Axflow
provider_slug: axflow
slug: axflow-domain-security
source_filename: axflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axflow.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 04:37:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: axflow.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axflow/refs/heads/main/security/axflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Tooling
- Platform
- LLM
---
