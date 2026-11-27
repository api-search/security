---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: pagosaforestlodge.com
  spf: true
hosts:
- cert_expires: Jan 28 20:38:09 2027 GMT
  host: pagosaforestlodge.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pagosa Forest Lodge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pagosa Forest Lodge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pagosa Forest Lodge
provider_slug: pagosaforestlodge-com
slug: pagosaforestlodge-com-domain-security
source_filename: pagosaforestlodge-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pagosaforestlodge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 20:38:09 2027 GMT\n  hsts: false\ndomains:\n- domain: pagosaforestlodge.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/pagosaforestlodge-com/security/pagosaforestlodge-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Cabin
- Luxury
- Colorado
- Vacation Rentals
- HotTub
---
