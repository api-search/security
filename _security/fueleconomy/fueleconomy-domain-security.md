---
api_specs:
- filename: fueleconomy-fuel-economy-web-services-openapi.yml
  format: yaml
  label: Fuel Economy Web Services
  slug: fuel-economy-web-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fueleconomy/refs/heads/main/openapi/fueleconomy-fuel-economy-web-services-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fueleconomy.gov
  spf: true
hosts:
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: www.fueleconomy.gov
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Fueleconomy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FuelEconomy.gov, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: FuelEconomy.gov
provider_slug: fueleconomy
slug: fueleconomy-domain-security
source_filename: fueleconomy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fueleconomy.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: fueleconomy.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fueleconomy/refs/heads/main/security/fueleconomy-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Fuel Economy
- EPA
- DOE
- Energy
- Vehicles
- Emissions
- CO2
- MPG
- Automotive
- Government
- Open Data
---
