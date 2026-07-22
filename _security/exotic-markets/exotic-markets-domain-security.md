---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: exotic.markets
  spf: true
hosts:
- cert_expires: Oct 16 19:30:03 2026 GMT
  host: exotic.markets
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exotic Markets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exotic Markets, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Exotic Markets
provider_slug: exotic-markets
slug: exotic-markets-domain-security
source_filename: exotic-markets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: exotic.markets\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 19:30:03 2026 GMT\n  hsts: false\ndomains:\n- domain: exotic.markets\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exotic-markets/refs/heads/main/security/exotic-markets-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Crypto Web3
- DeFi
- Solana
- Options
- Structured Products
- Derivatives
- Blockchain
---
