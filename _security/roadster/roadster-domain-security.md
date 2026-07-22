---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: roadster.com
  spf: true
hosts:
- cert_expires: Sep 14 15:55:43 2026 GMT
  host: roadster.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Roadster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for roadster, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: roadster
provider_slug: roadster
slug: roadster-domain-security
source_filename: roadster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: roadster.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:55:43 2026 GMT\n  hsts: false\ndomains:\n- domain: roadster.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roadster/refs/heads/main/security/roadster-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automotive
- Digital Retail
- Commerce
- E-Commerce
- Dealership
- Acquired
---
