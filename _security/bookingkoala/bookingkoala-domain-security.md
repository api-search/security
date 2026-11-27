---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bookingkoala.com
  spf: true
hosts:
- cert_expires: Feb  3 21:07:02 2027 GMT
  host: www.bookingkoala.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BookingKoala Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BookingKoala, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BookingKoala
provider_slug: bookingkoala
slug: bookingkoala-domain-security
source_filename: bookingkoala-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bookingkoala.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 21:07:02 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: bookingkoala.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bookingkoala/security/bookingkoala-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Service Platform
- Booking
- Software-as-a-Service
- Business
- Automation
---
