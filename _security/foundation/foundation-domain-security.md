---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: thegraph.com
  spf: true
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:certmaster@alchemyapi.io"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: alchemyapi.io
  spf: true
hosts:
- cert_expires: Oct  6 21:32:21 2026 GMT
  host: thegraph.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 05:49:39 2026 GMT
  host: api.thegraph.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: eth-mainnet.alchemyapi.io
  https: false
kind: domain-security
layout: security
method: probed
name: Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Foundation, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Foundation
provider_slug: foundation
slug: foundation-domain-security
source_filename: foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thegraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:32:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.thegraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 05:49:39 2026 GMT\n  hsts: null\n- host: eth-mainnet.alchemyapi.io\n  https: false\ndomains:\n- domain: thegraph.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: alchemyapi.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:certmaster@alchemyapi.io\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com;\
  \ cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/foundation/refs/heads/main/security/foundation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- NFT
- Digital Art
- Marketplace
- Ethereum
- Web3
- Blockchain
- Creators
- Auctions
- Collectors
---
