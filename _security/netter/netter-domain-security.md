---
api_specs:
- filename: netter-openapi-original.json
  format: json
  label: Netter API (DMI Backend)
  slug: netter-api-dmi-backend
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netter/refs/heads/main/openapi/netter-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: netter.ai
  spf: false
hosts:
- cert_expires: Aug 27 20:16:48 2026 GMT
  host: www.netter.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 17:15:55 2026 GMT
  host: netter.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: api.netter.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Netter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Netter, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Netter
provider_slug: netter
slug: netter-domain-security
source_filename: netter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.netter.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 20:16:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: netter.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 17:15:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.netter.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: netter.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netter/refs/heads/main/security/netter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- Data Platform
- Analytics
- Artificial Intelligence
- Ontology
- Data Integration
- Pipelines
- ETL
- Y Combinator
---
