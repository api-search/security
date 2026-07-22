---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: remitbee.com
  spf: true
hosts:
- cert_expires: Oct 18 14:05:59 2026 GMT
  host: remitbee.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Remitbee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Remitbee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Remitbee
provider_slug: remitbee
slug: remitbee-domain-security
source_filename: remitbee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: remitbee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 14:05:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: remitbee.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remitbee/refs/heads/main/security/remitbee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Money Transfer
- Remittances
- Currency Exchange
- Payments
- Fintech
- Cross-Border Payments
- Mobile Top-Up
- Bill Payment
- Canada
---
