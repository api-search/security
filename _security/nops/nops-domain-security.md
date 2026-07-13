---
api_specs:
- filename: nops-nops-openapi.yml
  format: yaml
  label: nOps
  slug: nops
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nops/refs/heads/main/openapi/nops-nops-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nops.io
  spf: true
hosts:
- cert_expires: Oct  9 03:22:51 2026 GMT
  host: www.nops.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  7 01:36:52 2026 GMT
  host: app.nops.io
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nops Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for nOps, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: nOps
provider_slug: nops
slug: nops-domain-security
source_filename: nops-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nops.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 03:22:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.nops.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  7 01:36:52 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: nops.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nops/refs/heads/main/security/nops-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Costs
- FinOps
---
