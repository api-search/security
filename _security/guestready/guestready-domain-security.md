---
api_specs:
- filename: guestready-rentalready-openapi.yml
  format: yaml
  label: RentalReady API
  slug: rentalready-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guestready/refs/heads/main/openapi/guestready-rentalready-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: guestready.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rentalready.io
  spf: true
hosts:
- cert_expires: Oct 31 23:48:55 2026 GMT
  host: www.guestready.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 19:05:07 2026 GMT
  host: pms.rentalready.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Guestready Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GuestReady, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GuestReady
provider_slug: guestready
slug: guestready-domain-security
source_filename: guestready-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.guestready.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:48:55 2026 GMT\n  hsts: false\n- host: pms.rentalready.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 19:05:07 2026 GMT\n  hsts: false\ndomains:\n- domain: guestready.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rentalready.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guestready/refs/heads/main/security/guestready-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Property Management
- Short Term Rentals
- Vacation Rentals
- Hospitality
- Travel
- Real Estate
- Channel Management
- Reservations
- Revenue Management
- PMS
- MCP
- OAuth
---
