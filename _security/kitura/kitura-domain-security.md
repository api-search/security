---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: kitura.dev
  spf: true
hosts:
- cert_expires: Sep 22 13:01:22 2026 GMT
  host: www.kitura.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kitura Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kitura, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kitura
provider_slug: kitura
slug: kitura-domain-security
source_filename: kitura-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kitura.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 13:01:22 2026 GMT\n  hsts: false\ndomains:\n- domain: kitura.dev\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kitura/refs/heads/main/security/kitura-domain-security.yml
summary_line: TLSv1.3
tags:
- Archived
- Deployment
- Frameworks
- Server-Side Swift
- Web
---
