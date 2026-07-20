---
api_specs:
- filename: gentrace-openapi-original.json
  format: json
  label: Gentrace API
  slug: gentrace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gentrace/refs/heads/main/openapi/gentrace-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gentrace.ai
  spf: true
hosts:
- cert_expires: Oct  9 20:11:42 2026 GMT
  host: gentrace.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gentrace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gentrace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gentrace
provider_slug: gentrace
slug: gentrace-domain-security
source_filename: gentrace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gentrace.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 20:11:42 2026 GMT\n  hsts: false\ndomains:\n- domain: gentrace.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gentrace/refs/heads/main/security/gentrace-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- LLM
- Evaluation
- Testing
- Observability
- Machine Learning
- Developer Tools
---
