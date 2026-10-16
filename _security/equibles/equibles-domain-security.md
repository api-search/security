---
api_specs:
- filename: equibles-openapi-generated.yml
  format: yaml
  label: Equibles API
  slug: equibles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equibles/refs/heads/main/openapi/_ae-authored/equibles-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: equibles.com
  spf: true
hosts:
- cert_expires: Nov  6 23:26:28 2026 GMT
  host: equibles.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Equibles Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Equibles, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Equibles
provider_slug: equibles
slug: equibles-domain-security
source_filename: equibles-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: equibles.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:26:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: equibles.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/equibles/refs/heads/main/security/equibles-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Finance
- Data
- API
- Stocks
---
