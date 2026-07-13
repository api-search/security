---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kaiko.com
  spf: true
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: false
  dnssec: false
  domain: kaiko.io
  spf: false
hosts:
- cert_expires: Aug 30 10:53:54 2026 GMT
  host: www.kaiko.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 15:40:31 2026 GMT
  host: docs.kaiko.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 02:27:14 2026 GMT
  host: us.market-api.kaiko.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kaiko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kaiko, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kaiko
provider_slug: kaiko
slug: kaiko-domain-security
source_filename: kaiko-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kaiko.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 10:53:54 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: docs.kaiko.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 15:40:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: us.market-api.kaiko.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 02:27:14 2026 GMT\n  hsts: null\ndomains:\n- domain: kaiko.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: kaiko.io\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kaiko/refs/heads/main/security/kaiko-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web3
- Crypto
- Market Data
- Institutional
- FX
- Indices
- On-Chain
- Streaming
---
