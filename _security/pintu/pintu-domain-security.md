---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pintu.co.id
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: pintu.pro
  spf: false
hosts:
- cert_expires: Oct 11 09:40:01 2026 GMT
  host: pintu.co.id
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: docs.pintu.pro
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: partner.pintu.co.id
  https: false
kind: domain-security
layout: security
method: probed
name: Pintu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pintu, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Pintu
provider_slug: pintu
slug: pintu-domain-security
source_filename: pintu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pintu.co.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 09:40:01 2026 GMT\n  hsts: false\n- host: docs.pintu.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: null\n- host: partner.pintu.co.id\n  https: false\ndomains:\n- domain: pintu.co.id\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: pintu.pro\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pintu/refs/heads/main/security/pintu-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Crypto Exchange
- Trading
- Fintech
- Digital Assets
- Web3
- Indonesia
- WebSocket
- Institutional Trading
---
