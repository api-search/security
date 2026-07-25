---
api_specs:
- filename: anduril-entities-api-openapi.yml
  format: yaml
  label: Anduril Industries Entities API
  slug: anduril-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anduril/refs/heads/main/openapi/anduril-entities-api-openapi.yml
- filename: anduril-oauth-api-openapi.yml
  format: yaml
  label: Anduril Industries OAuth API
  slug: anduril-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anduril/refs/heads/main/openapi/anduril-oauth-api-openapi.yml
- filename: anduril-objects-api-openapi.yml
  format: yaml
  label: Anduril Industries Objects API
  slug: anduril-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anduril/refs/heads/main/openapi/anduril-objects-api-openapi.yml
- filename: anduril-tasks-api-openapi.yml
  format: yaml
  label: Anduril Industries Tasks API
  slug: anduril-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anduril/refs/heads/main/openapi/anduril-tasks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: anduril.com
  spf: true
hosts:
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: www.anduril.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: developer.anduril.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anduril Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anduril Industries, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Anduril Industries
provider_slug: anduril
slug: anduril-domain-security
source_filename: anduril-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anduril.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: false\n- host: developer.anduril.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: anduril.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anduril/refs/heads/main/security/anduril-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Defense
- Autonomy
- Lattice
- Command and Control
- C2
- Sensors
- Effectors
- Counter-UAS
- Unmanned Systems
- Mission Software
- Edge AI
- ITAR
---
