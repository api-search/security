---
api_specs:
- filename: clyde-openapi-generated.yml
  format: yaml
  label: Clyde API
  slug: clyde-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clyde/refs/heads/main/openapi/_ae-authored/clyde-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: joinclyde.com
  spf: true
hosts:
- cert_expires: Dec 12 14:35:30 2026 GMT
  host: joinclyde.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clyde Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clyde, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clyde
provider_slug: clyde
slug: clyde-domain-security
source_filename: clyde-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: joinclyde.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 14:35:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: joinclyde.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clyde/refs/heads/main/security/clyde-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Extended Warranty
- Product Registration
- Shipping Protection
- E‑commerce Integration
- Claims Processing
---
