---
api_specs:
- filename: lokki-external-api-openapi.json
  format: json
  label: Lokki External API
  slug: lokki-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lokki/refs/heads/main/openapi/lokki-external-api-openapi.json
- filename: lokki-dashboard-api-openapi.json
  format: json
  label: Lokki Dashboard API
  slug: lokki-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lokki/refs/heads/main/openapi/lokki-dashboard-api-openapi.json
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lokki.rent
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getlokki.com
  spf: true
hosts:
- cert_expires: Sep 26 04:38:56 2026 GMT
  host: www.lokki.rent
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 17:14:52 2026 GMT
  host: solutions.lokki.rent
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 21:20:02 2026 GMT
  host: docs.getlokki.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lokki Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lokki, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Lokki
provider_slug: lokki
slug: lokki-domain-security
source_filename: lokki-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lokki.rent\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 04:38:56 2026 GMT\n  hsts: null\n- host: solutions.lokki.rent\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 17:14:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.getlokki.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 21:20:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lokki.rent\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: getlokki.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lokki/refs/heads/main/security/lokki-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Climate Tech
- Circular Economy
- Rental
- Equipment Rental
- Bike Rental
- Marketplace
- Booking
- Reservations
- Inventory
- Catalog
- Pricing
- Availability
- Mobility
- Outdoor Recreation
- Point of Sale
- SaaS
- France
- MCP
- Agents
- Agent Skills
---
