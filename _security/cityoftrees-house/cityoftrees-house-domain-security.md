---
api_specs:
- filename: cityoftrees-house-agent-api-openapi.yml
  format: yaml
  label: City of Trees House Agent API
  slug: cityoftrees-house-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cityoftrees-house/openapi/cityoftrees-house-agent-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cityoftrees.house
  spf: true
hosts:
- cert_expires: Jan 14 15:57:32 2027 GMT
  host: cityoftrees.house
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: City of Trees House Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for City of Trees House, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: City of Trees House
provider_slug: cityoftrees-house
slug: cityoftrees-house-domain-security
source_filename: cityoftrees-house-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cityoftrees.house\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 15:57:32 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cityoftrees.house\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cityoftrees-house/security/cityoftrees-house-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Vacation Rentals
- West Sacramento
- Family Run
- Hospitality
- Vacation Home
---
