---
api_specs:
- filename: tock-reservation-openapi.yml
  format: yaml
  label: Tock Reservation API
  slug: reservation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tock/refs/heads/main/openapi/tock-reservation-openapi.yml
- filename: tock-guest-profile-openapi.yml
  format: yaml
  label: Tock Guest API
  slug: guest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tock/refs/heads/main/openapi/tock-guest-profile-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: exploretock.com
  spf: true
hosts:
- cert_expires: Sep  1 19:43:17 2026 GMT
  host: www.exploretock.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 19:43:17 2026 GMT
  host: api.exploretock.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tock, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Tock
provider_slug: tock
slug: tock-domain-security
source_filename: tock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.exploretock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 19:43:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.exploretock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 19:43:17 2026 GMT\n  hsts: null\ndomains:\n- domain: exploretock.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tock/refs/heads/main/security/tock-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Hospitality
- Reservations
- Restaurants
- Wineries
- Ticketed Events
- Takeout
- Delivery
- Experiences
- Dining
- American Express
---
