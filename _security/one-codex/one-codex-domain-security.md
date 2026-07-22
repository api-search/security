---
api_specs:
- filename: one-codex-openapi-original.json
  format: json
  label: One Codex API (v1)
  slug: one-codex-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/one-codex/refs/heads/main/openapi/one-codex-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: onecodex.com
  spf: true
hosts:
- cert_expires: Oct  6 10:14:41 2026 GMT
  host: app.onecodex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: One Codex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for One Codex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: One Codex
provider_slug: one-codex
slug: one-codex-domain-security
source_filename: one-codex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.onecodex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 10:14:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: onecodex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/one-codex/refs/heads/main/security/one-codex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Genomics
- Microbiome
- Bioinformatics
- Metagenomics
- Life Sciences
- Sequencing
- Healthcare
- Data Platform
- API
---
