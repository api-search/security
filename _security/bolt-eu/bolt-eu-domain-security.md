---
api_specs:
- filename: bolt-eu-genericclient-api-openapi.yml
  format: yaml
  label: Bolt GenericClient API
  slug: bolt-eu-genericclient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-eu/refs/heads/main/openapi/bolt-eu-genericclient-api-openapi.yml
- filename: bolt-eu-pim-api-openapi.yml
  format: yaml
  label: Bolt Pim API
  slug: bolt-eu-pim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-eu/refs/heads/main/openapi/bolt-eu-pim-api-openapi.yml
- filename: bolt-eu-validateloyaltycard-api-openapi.yml
  format: yaml
  label: Bolt ValidateLoyaltyCard API
  slug: bolt-eu-validateloyaltycard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-eu/refs/heads/main/openapi/bolt-eu-validateloyaltycard-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bolt.eu
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: bolt.eu
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  3 23:59:59 2027 GMT
  host: developer.bolt.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: node.bolt.eu
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bolt Eu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bolt, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bolt
provider_slug: bolt-eu
slug: bolt-eu-domain-security
source_filename: bolt-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bolt.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: developer.bolt.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: node.bolt.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bolt.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bolt-eu/refs/heads/main/security/bolt-eu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Ride Booking
- Ride Hailing
- Mobility
- Transportation
- Food Delivery
- Micromobility
- Delivery
- Super App
---
