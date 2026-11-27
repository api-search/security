---
api_specs:
- filename: carchat-io-dealers-api-openapi.yml
  format: yaml
  label: CarChat Dealers API
  slug: carchat-io-dealers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carchat-io/openapi/carchat-io-dealers-api-openapi.yml
- filename: carchat-io-inventory-api-openapi.yml
  format: yaml
  label: CarChat Inventory API
  slug: carchat-io-inventory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carchat-io/openapi/carchat-io-inventory-api-openapi.yml
- filename: carchat-io-lead-api-openapi.yml
  format: yaml
  label: CarChat Lead API
  slug: carchat-io-lead-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carchat-io/openapi/carchat-io-lead-api-openapi.yml
- filename: carchat-io-segments-api-openapi.yml
  format: yaml
  label: CarChat Segments API
  slug: carchat-io-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carchat-io/openapi/carchat-io-segments-api-openapi.yml
- filename: carchat-io-vehicles-api-openapi.yml
  format: yaml
  label: CarChat Vehicles API
  slug: carchat-io-vehicles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carchat-io/openapi/carchat-io-vehicles-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: carchat.io
  spf: true
hosts:
- cert_expires: Jan 29 17:14:33 2027 GMT
  host: carchat.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CarChat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CarChat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CarChat
provider_slug: carchat-io
slug: carchat-io-domain-security
source_filename: carchat-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carchat.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 17:14:33 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: carchat.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/carchat-io/security/carchat-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketplace
- Automotive
- Artificial Intelligence
- OpenAPI
---
