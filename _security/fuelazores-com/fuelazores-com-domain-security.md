---
api_specs:
- filename: fuelazores-com-articles-api-openapi.yml
  format: yaml
  label: FuelAzores Articles API
  slug: fuelazores-com-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fuelazores-com/openapi/fuelazores-com-articles-api-openapi.yml
- filename: fuelazores-com-history-api-openapi.yml
  format: yaml
  label: FuelAzores History API
  slug: fuelazores-com-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fuelazores-com/openapi/fuelazores-com-history-api-openapi.yml
- filename: fuelazores-com-prices-api-openapi.yml
  format: yaml
  label: FuelAzores Prices API
  slug: fuelazores-com-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fuelazores-com/openapi/fuelazores-com-prices-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: fuelazores.com
  spf: false
hosts:
- cert_expires: Dec 27 21:53:33 2026 GMT
  host: fuelazores.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FuelAzores Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FuelAzores, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: FuelAzores
provider_slug: fuelazores-com
slug: fuelazores-com-domain-security
source_filename: fuelazores-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fuelazores.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 21:53:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fuelazores.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fuelazores-com/security/fuelazores-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Energy
- Fuel
- Prices
- Portugal
---
