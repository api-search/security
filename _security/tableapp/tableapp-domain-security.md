---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:wenchen.x@gmail.com"
  - 0 issue ";"
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: tableapp.com
  spf: true
hosts:
- cert_expires: Oct  6 16:27:13 2026 GMT
  host: tableapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tableapp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TableApp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TableApp
provider_slug: tableapp
slug: tableapp-domain-security
source_filename: tableapp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tableapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 16:27:13 2026 GMT\n  hsts: false\ndomains:\n- domain: tableapp.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:wenchen.x@gmail.com\"\n  - 0 issue \";\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tableapp/refs/heads/main/security/tableapp-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Restaurants
- Reservations
- Restaurant Booking
- Hospitality
- Food and Dining
- Consumer
- Malaysia
---
