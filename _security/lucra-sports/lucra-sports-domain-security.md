---
api_specs:
- filename: lucra-sports-forge-openapi.json
  format: json
  label: Lucra Forge API
  slug: lucra-sports-forge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucra-sports/refs/heads/main/openapi/lucra-sports-forge-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: playlucra.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lucrasports.com
  spf: true
hosts:
- cert_expires: Oct  6 11:32:33 2026 GMT
  host: www.playlucra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 04:56:01 2026 GMT
  host: docs.lucrasports.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: forge.lucrasports.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lucra Sports Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lucra Sports, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lucra Sports
provider_slug: lucra-sports
slug: lucra-sports-domain-security
source_filename: lucra-sports-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.playlucra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 11:32:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.lucrasports.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 04:56:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: forge.lucrasports.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: playlucra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: lucrasports.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucra-sports/refs/heads/main/security/lucra-sports-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Gaming
- Sports
- Gamification
- Loyalty
- Tournaments
- Contests
- Payments
- Wagering
- Embedded Finance
- SDKs
- Webhooks
- Compliance
---
