---
api_specs:
- filename: openapi.json
  format: json
  label: Evidently Platform REST API
  slug: evidently-platform-rest-api
  spec_type: OpenAPI
  url: https://docs.evidentlyai.com/api-reference/openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: evidentlyai.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: evidently.cloud
  spf: false
hosts:
- cert_expires: Sep 11 23:38:54 2026 GMT
  host: www.evidentlyai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 20:30:14 2026 GMT
  host: docs.evidentlyai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 09:32:44 2026 GMT
  host: app.evidently.cloud
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evidently Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evidently AI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Evidently AI
provider_slug: evidently
slug: evidently-domain-security
source_filename: evidently-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.evidentlyai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:38:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.evidentlyai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 20:30:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.evidently.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 09:32:44 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: evidentlyai.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: evidently.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evidently/refs/heads/main/security/evidently-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ML Monitoring
- LLM Observability
- Data Drift
- Model Performance
- AI Evaluation
- Data Quality
- Open Source
- MLOps
- LLMOps
- Generative AI
---
