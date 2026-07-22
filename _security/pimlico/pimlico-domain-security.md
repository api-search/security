---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pimlico.io
  spf: true
hosts:
- cert_expires: Sep  9 17:50:02 2026 GMT
  host: www.pimlico.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 01:30:05 2026 GMT
  host: docs.pimlico.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 18:40:26 2026 GMT
  host: api.pimlico.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pimlico Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pimlico, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Pimlico
provider_slug: pimlico
slug: pimlico-domain-security
source_filename: pimlico-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pimlico.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 17:50:02 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.pimlico.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 01:30:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.pimlico.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 18:40:26 2026 GMT\n  hsts: null\ndomains:\n- domain: pimlico.io\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pimlico/refs/heads/main/security/pimlico-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Account Abstraction
- ERC-4337
- Blockchain
- Ethereum
- Web3
- Paymaster
- Bundler
- Smart Accounts
- Gas Sponsorship
- Wallets
- Infrastructure
---
