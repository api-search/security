---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rentals.ca
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rentsync.ca
  spf: true
hosts:
- cert_expires: Oct 18 19:19:50 2026 GMT
  host: rentals.ca
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 05:31:31 2026 GMT
  host: partners.rentsync.ca
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 01:59:22 2026 GMT
  host: rentsync.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rentals Ca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rentals.ca, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rentals.ca
provider_slug: rentals-ca
slug: rentals-ca-domain-security
source_filename: rentals-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rentals.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 19:19:50 2026 GMT\n  hsts: null\n- host: partners.rentsync.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 05:31:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: rentsync.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 01:59:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rentals.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: rentsync.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rentals-ca/refs/heads/main/security/rentals-ca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Canada
- Rentals
- Property Listings
- Rental Marketplace
- PropTech
- Listing Syndication
- Market Data
---
