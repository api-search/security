---
api_specs:
- filename: starfish-data-platform-openapi.yml
  format: yaml
  label: Itron Starfish Data Platform API
  slug: itron-starfish-data-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itron/refs/heads/main/openapi/starfish-data-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: itron.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: ssni.com
  spf: true
hosts:
- cert_expires: Oct  4 14:47:00 2026 GMT
  host: na.itron.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 14:47:00 2026 GMT
  host: partner.itron.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.ssni.com
  https: false
kind: domain-security
layout: security
method: probed
name: Itron Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Itron, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Itron
provider_slug: itron
slug: itron-domain-security
source_filename: itron-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: na.itron.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 14:47:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: partner.itron.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 14:47:00 2026 GMT\n  hsts: null\n- host: developer.ssni.com\n  https: false\ndomains:\n- domain: itron.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ssni.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itron/refs/heads/main/security/itron-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Itron
- Utilities
- Smart Meters
- Smart Grid
- Smart Cities
- Internet Of Things
- IoT
- Energy
- Water
- Gas
- Electricity
- Distributed Intelligence
- Grid Edge
- AMI
- AMR
- RF Mesh
- IPv6
- OData
- Industrial IoT
- Fortune 1000
- NASDAQ ITRI
---
