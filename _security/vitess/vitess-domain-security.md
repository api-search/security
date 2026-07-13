---
api_specs:
- filename: vitess-vtadmin-openapi.yml
  format: yaml
  label: Vitess VTAdmin API
  slug: vtadmin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vitess/refs/heads/main/openapi/vitess-vtadmin-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vitess.io
  spf: true
hosts:
- cert_expires: Aug 14 10:03:47 2026 GMT
  host: vitess.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vitess Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vitess, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vitess
provider_slug: vitess
slug: vitess-domain-security
source_filename: vitess-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vitess.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 10:03:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vitess.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vitess/refs/heads/main/security/vitess-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Native
- CNCF
- Database
- Distributed Systems
- Graduated
- MySQL
- Sharding
---
