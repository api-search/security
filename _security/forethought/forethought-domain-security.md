---
api_specs:
- filename: forethought-solve-api-openapi.yml
  format: yaml
  label: Forethought Solve API
  slug: forethought-solve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forethought/refs/heads/main/openapi/forethought-solve-api-openapi.yml
- filename: forethought-triage-api-openapi.yml
  format: yaml
  label: Forethought Triage API
  slug: forethought-triage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forethought/refs/heads/main/openapi/forethought-triage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: forethought.ai
  spf: true
hosts:
- cert_expires: Sep 30 02:24:14 2026 GMT
  host: forethought.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:48:48 2026 GMT
  host: support.forethought.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 05:32:41 2026 GMT
  host: app.forethought.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Forethought Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forethought, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Forethought
provider_slug: forethought
slug: forethought-domain-security
source_filename: forethought-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forethought.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 02:24:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.forethought.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:48:48 2026 GMT\n  hsts: false\n- host: app.forethought.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 05:32:41 2026 GMT\n  hsts: null\ndomains:\n- domain: forethought.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forethought/refs/heads/main/security/forethought-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Artificial Intelligence
- Customer Support
- Customer Service
- Generative AI
- SupportGPT
- Conversational AI
- Ticket Triage
- Agentic AI
- Voice AI
- Helpdesk
- Multi-Agent
---
