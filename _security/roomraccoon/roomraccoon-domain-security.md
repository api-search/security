---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: roomraccoon.com
  spf: true
hosts:
- cert_expires: Sep  9 11:01:31 2026 GMT
  host: roomraccoon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Roomraccoon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RoomRaccoon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: RoomRaccoon
provider_slug: roomraccoon
slug: roomraccoon-domain-security
source_filename: roomraccoon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: roomraccoon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 11:01:31 2026 GMT\n  hsts: false\ndomains:\n- domain: roomraccoon.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roomraccoon/refs/heads/main/security/roomraccoon-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Hospitality
- Hotels
- Hotel Management
- Property Management System
- PMS
- Channel Manager
- Booking Engine
- Payments
- Revenue Management
- Independent Hotels
- Bed And Breakfast
- Guesthouse
- Travel
- SaaS
---
