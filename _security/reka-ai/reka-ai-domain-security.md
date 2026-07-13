---
api_specs:
- filename: reka-ai-openapi.yml
  format: yaml
  label: Reka AI Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reka-ai/refs/heads/main/openapi/reka-ai-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: reka.ai
  spf: true
hosts:
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: www.reka.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 15:15:03 2026 GMT
  host: docs.reka.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 19:37:59 2026 GMT
  host: api.reka.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reka Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reka AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Reka AI
provider_slug: reka-ai
slug: reka-ai-domain-security
source_filename: reka-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reka.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.reka.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 15:15:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.reka.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 19:37:59 2026 GMT\n  hsts: null\ndomains:\n- domain: reka.ai\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reka-ai/refs/heads/main/security/reka-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Inference
- Multimodal
- Foundation Models
- Vision
---
