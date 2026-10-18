---
api_specs:
- filename: codewords-workflows-api-openapi.yml
  format: yaml
  label: Agemo Workflows API
  slug: codewords-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codewords/refs/heads/main/openapi/codewords-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: codewords.ai
  spf: true
hosts:
- cert_expires: Nov 27 10:38:48 2026 GMT
  host: codewords.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Codewords Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agemo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Agemo
provider_slug: codewords
slug: codewords-domain-security
source_filename: codewords-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codewords.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 10:38:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: codewords.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codewords/refs/heads/main/security/codewords-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Automation
- Workflows
- No-Code
- Software-as-a-Service
- Productivity
---
