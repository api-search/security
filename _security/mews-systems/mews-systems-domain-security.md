---
api_specs:
- filename: swagger.yaml
  format: yaml
  label: Mews Connector API
  slug: mews-connector-api
  spec_type: OpenAPI
  url: https://api.mews.com/Swagger/connector/swagger.yaml
- filename: swagger.yaml
  format: yaml
  label: Mews Booking Engine API
  slug: mews-booking-engine-api
  spec_type: OpenAPI
  url: https://api.mews.com/Swagger/distributor/swagger.yaml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 Issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mews.com
  spf: true
hosts:
- cert_expires: Sep 21 01:01:40 2026 GMT
  host: www.mews.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 17:58:02 2026 GMT
  host: developers.mews.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 18:53:59 2026 GMT
  host: docs.mews.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mews Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mews, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Mews
provider_slug: mews-systems
slug: mews-systems-domain-security
source_filename: mews-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mews.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 01:01:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.mews.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 17:58:02 2026 GMT\n  hsts: false\n- host: docs.mews.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 18:53:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mews.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 Issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mews-systems/refs/heads/main/security/mews-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Hospitality
- Hotel
- Property Management
- PMS
- Reservations
- Bookings
- Travel
- Payments
- Point of Sale
- Channel Manager
- Booking Engine
---
