---
api_specs:
- filename: cherre-openapi.yml
  format: yaml
  label: Cherre Property API
  slug: property
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cherre/refs/heads/main/openapi/cherre-openapi.yml
- filename: cherre-openapi.yml
  format: yaml
  label: Cherre Tax Assessor API
  slug: tax-assessor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cherre/refs/heads/main/openapi/cherre-openapi.yml
- filename: cherre-openapi.yml
  format: yaml
  label: Cherre Recorder API
  slug: recorder
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cherre/refs/heads/main/openapi/cherre-openapi.yml
- filename: cherre-openapi.yml
  format: yaml
  label: Cherre Owner & Parcel API
  slug: owner-parcel
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cherre/refs/heads/main/openapi/cherre-openapi.yml
- filename: cherre-openapi.yml
  format: yaml
  label: Cherre Connections API
  slug: connections
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cherre/refs/heads/main/openapi/cherre-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cherre.com
  spf: true
hosts:
- cert_expires: Aug 20 12:10:46 2026 GMT
  host: www.cherre.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 01:12:53 2026 GMT
  host: cherre.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- host: api.cherre.com
  https: false
kind: domain-security
layout: security
method: probed
name: Cherre Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cherre, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cherre
provider_slug: cherre
slug: cherre-domain-security
source_filename: cherre-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cherre.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 12:10:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: cherre.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 01:12:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: api.cherre.com\n  https: false\ndomains:\n- domain: cherre.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cherre/refs/heads/main/security/cherre-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Property Intelligence
- Data Integration
- Knowledge Graph
- GraphQL
---
