---
api_specs:
- filename: looksrare-openapi.json
  format: json
  label: LooksRare Orders API
  slug: orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looksrare/refs/heads/main/openapi/looksrare-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: looksrare.org
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: looksrare.dev
  spf: true
hosts:
- cert_expires: Aug 16 20:24:58 2026 GMT
  host: looksrare.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 21:29:49 2026 GMT
  host: looksrare.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 20:24:58 2026 GMT
  host: api.looksrare.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Looksrare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LooksRare, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: LooksRare
provider_slug: looksrare
slug: looksrare-domain-security
source_filename: looksrare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: looksrare.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 20:24:58 2026 GMT\n  hsts: null\n- host: looksrare.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 21:29:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.looksrare.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 20:24:58 2026 GMT\n  hsts: null\ndomains:\n- domain: looksrare.org\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: looksrare.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/looksrare/refs/heads/main/security/looksrare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- NFT
- Marketplace
- Ethereum
- Web3
- Orders
- Collections
- Tokens
- Events
- ERC-721
- ERC-1155
- Seaport
- Community
---
