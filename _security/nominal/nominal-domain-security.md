---
api_specs:
- filename: nominal-openapi-generated.yml
  format: yaml
  label: Nominal API
  slug: nominal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nominal/openapi/_ae-authored/nominal-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nominal.io
  spf: true
hosts:
- cert_expires: Feb  5 04:42:56 2027 GMT
  host: nominal.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 19:02:03 2027 GMT
  host: docs.nominal.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 13:47:27 2026 GMT
  host: api.gov.nominal.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Nominal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nominal, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Nominal
provider_slug: nominal
slug: nominal-domain-security
source_filename: nominal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nominal.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 04:42:56 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.nominal.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 19:02:03 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.gov.nominal.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 13:47:27 2026 GMT\n  hsts: null\ndomains:\n- domain: nominal.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/nominal/security/nominal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Deep Tech
- Test and Measurement
- Hardware
- Aerospace
- Telemetry
- Observability
- Industrial Data
- Data Platform
- SDK
---
