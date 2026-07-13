---
api_specs:
- filename: log10-logging-openapi.yml
  format: yaml
  label: Log10 LLM Logging API
  slug: log10-llm-logging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/log10/refs/heads/main/openapi/log10-logging-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: log10.io
  spf: true
hosts:
- cert_expires: Sep 20 23:56:46 2026 GMT
  host: log10.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: docs.log10.io
  https: false
kind: domain-security
layout: security
method: probed
name: Log10 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Log10, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Log10
provider_slug: log10
slug: log10-domain-security
source_filename: log10-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: log10.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:56:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.log10.io\n  https: false\ndomains:\n- domain: log10.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/log10/refs/heads/main/security/log10-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- LLM
- Logging
- Observability
- Evaluation
- Feedback
- Debugging
- LLMOps
- Artificial Intelligence
- Machine Learning
---
