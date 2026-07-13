---
api_specs:
- filename: octopus-energy-public-api-openapi.yml
  format: yaml
  label: Octopus Energy Public API
  slug: octopus-energy-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octopus-energy/refs/heads/main/openapi/octopus-energy-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: octopus.energy
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kraken.tech
  spf: true
hosts:
- cert_expires: Sep 19 20:52:54 2026 GMT
  host: octopus.energy
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: developer.octopus.energy
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 00:40:57 2026 GMT
  host: kraken.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Octopus Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Octopus Energy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Octopus Energy
provider_slug: octopus-energy
slug: octopus-energy-domain-security
source_filename: octopus-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: octopus.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 20:52:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.octopus.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: false\n- host: kraken.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 00:40:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: octopus.energy\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: kraken.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octopus-energy/refs/heads/main/security/octopus-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Electricity
- Gas
- Renewable Energy
- Smart Meter
- Tariffs
- Kraken
- UK
- DER
- Electric Vehicles
- Heat Pumps
- Solar
- Battery
---
