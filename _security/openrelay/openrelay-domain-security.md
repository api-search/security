---
api_specs:
- filename: openrelay-openapi.json
  format: json
  label: OpenRelay API (control-plane)
  slug: openrelay-api-control-plane
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrelay/refs/heads/main/openapi/openrelay-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openrelay.inc
  spf: false
hosts:
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: api.openrelay.inc
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: api.beta.openrelay.inc
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openrelay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenRelay, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: OpenRelay
provider_slug: openrelay
slug: openrelay-domain-security
source_filename: openrelay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.openrelay.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: null\n- host: api.beta.openrelay.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: openrelay.inc\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openrelay/refs/heads/main/security/openrelay-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- GPU
- Inference
- AI
- Machine Learning
- Cloud Compute
- Infrastructure
- OpenAI-Compatible
- GPU Cloud
- LLM
---
