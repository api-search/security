---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: enigmalabs.io
  spf: true
hosts:
- cert_expires: Sep 17 17:56:10 2026 GMT
  host: enigmalabs.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Enigmalabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enigmalabs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Enigmalabs
provider_slug: enigmalabs
slug: enigmalabs-domain-security
source_filename: enigmalabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: enigmalabs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 17:56:10 2026 GMT\n  hsts: false\ndomains:\n- domain: enigmalabs.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enigmalabs/refs/heads/main/security/enigmalabs-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- UAP
- UFO
- Aerial Intelligence
- Crowdsourcing
- Mobile App
- Consumer
- Data Science
---
