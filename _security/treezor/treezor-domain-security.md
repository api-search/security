---
api_specs:
- filename: treezor-openapi-generated.yml
  format: yaml
  label: Treezor API
  slug: treezor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treezor/refs/heads/main/openapi/_ae-authored/treezor-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: treezor.com
  spf: true
hosts:
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: www.treezor.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Treezor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Treezor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Treezor
provider_slug: treezor
slug: treezor-domain-security
source_filename: treezor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.treezor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: treezor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treezor/refs/heads/main/security/treezor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- FinTech
- Payments
- Banking-as-a-Service
- API
- Europe
---
