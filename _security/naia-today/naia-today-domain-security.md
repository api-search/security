---
api_specs:
- filename: naia-today-v1-openapi.json
  format: json
  label: naia API V1 API
  slug: naia-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/naia-today/openapi/_original/naia-today-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: naia.today
  spf: true
hosts:
- cert_expires: Jan 12 15:12:02 2027 GMT
  host: naia.today
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Naia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Naia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Naia
provider_slug: naia-today
slug: naia-today-domain-security
source_filename: naia-today-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: naia.today\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 15:12:02 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: naia.today\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/naia-today/security/naia-today-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- SEO
- Geo
- Content
- Marketing
---
