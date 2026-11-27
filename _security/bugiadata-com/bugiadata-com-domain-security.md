---
api_specs:
- filename: bugiadata-com-api-openapi.yml
  format: yaml
  label: BugiaData Api API
  slug: bugiadata-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugiadata-com/openapi/_original/bugiadata-com-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bugiadata.com
  spf: true
hosts:
- cert_expires: Dec 14 19:02:59 2026 GMT
  host: bugiadata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BugiaData Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BugiaData, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BugiaData
provider_slug: bugiadata-com
slug: bugiadata-com-domain-security
source_filename: bugiadata-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bugiadata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 19:02:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bugiadata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bugiadata-com/security/bugiadata-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data
- Artificial Intelligence
- Testing
- Fake Data
---
