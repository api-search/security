---
api_specs:
- filename: shiprust-account-api-openapi.yml
  format: yaml
  label: ShipRust Account API
  slug: shiprust-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shiprust/openapi/shiprust-account-api-openapi.yml
- filename: shiprust-projects-api-openapi.yml
  format: yaml
  label: ShipRust Projects API
  slug: shiprust-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shiprust/openapi/shiprust-projects-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shiprust.com
  spf: true
hosts:
- cert_expires: Jan  3 18:27:01 2027 GMT
  host: shiprust.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Shiprust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShipRust, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ShipRust
provider_slug: shiprust
slug: shiprust-domain-security
source_filename: shiprust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shiprust.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 18:27:01 2027 GMT\n  hsts: false\ndomains:\n- domain: shiprust.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/shiprust/security/shiprust-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Rust
- SaaS
- Starter
- Axum
- PostgreSQL
---
