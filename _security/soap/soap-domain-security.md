---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: w3.org
  spf: true
hosts:
- cert_expires: Oct  7 03:48:25 2026 GMT
  host: www.w3.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Soap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SOAP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SOAP
provider_slug: soap
slug: soap-domain-security
source_filename: soap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.w3.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:48:25 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: w3.org\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soap/refs/heads/main/security/soap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SOAP
- Messaging Protocol
- Web Services
- XML
- W3C Standard
- Enterprise Integration
- WS-Star
---
