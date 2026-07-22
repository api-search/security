---
api_specs:
- filename: rapidata-openapi-original.json
  format: json
  label: Rapidata API
  slug: rapidata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rapidata/refs/heads/main/openapi/rapidata-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rapidata.ai
  spf: true
hosts:
- cert_expires: Oct 12 23:31:19 2026 GMT
  host: docs.rapidata.ai
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 04:36:56 2026 GMT
  host: api.rapidata.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rapidata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rapidata, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rapidata
provider_slug: rapidata
slug: rapidata-domain-security
source_filename: rapidata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.rapidata.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:31:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.rapidata.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 04:36:56 2026 GMT\n  hsts: null\ndomains:\n- domain: rapidata.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapidata/refs/heads/main/security/rapidata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Human Feedback
- Data Labeling
- Annotation
- RLHF
- Model Evaluation
- Machine Learning
- AI
- Crowdsourcing
- Preference Data
---
