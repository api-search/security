---
api_specs:
- filename: freeplay-openapi.yml
  format: yaml
  label: Freeplay Prompt Templates API
  slug: prompt-templates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/openapi/freeplay-openapi.yml
- filename: freeplay-openapi.yml
  format: yaml
  label: Freeplay Recordings & Sessions API
  slug: recordings-sessions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/openapi/freeplay-openapi.yml
- filename: freeplay-openapi.yml
  format: yaml
  label: Freeplay Test Cases & Datasets API
  slug: test-cases-datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/openapi/freeplay-openapi.yml
- filename: freeplay-openapi.yml
  format: yaml
  label: Freeplay Test Runs & Evaluations API
  slug: test-runs-evaluations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/openapi/freeplay-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: freeplay.ai
  spf: true
hosts:
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: freeplay.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 09:36:02 2026 GMT
  host: docs.freeplay.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 10:56:52 2026 GMT
  host: app.freeplay.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freeplay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freeplay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Freeplay
provider_slug: freeplay
slug: freeplay-domain-security
source_filename: freeplay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freeplay.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: null\n- host: docs.freeplay.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 09:36:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.freeplay.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 10:56:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: freeplay.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/security/freeplay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Evaluation
- Observability
- Prompt Management
- Experimentation
---
