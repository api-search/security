---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nftgo.io
  spf: true
hosts:
- cert_expires: Aug 22 09:42:00 2026 GMT
  host: nftgo.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 20:32:07 2026 GMT
  host: docs.nftgo.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 04:22:34 2026 GMT
  host: data-api.nftgo.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nftgo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NFTgo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NFTgo
provider_slug: nftgo
slug: nftgo-domain-security
source_filename: nftgo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nftgo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 09:42:00 2026 GMT\n  hsts: null\n- host: docs.nftgo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 20:32:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data-api.nftgo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 04:22:34 2026 GMT\n  hsts: null\ndomains:\n- domain: nftgo.io\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nftgo/refs/heads/main/security/nftgo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- NFT
- Blockchain
- Web3
- NFT Data
- NFT Analytics
- NFT Trading
- Market Data
- Cryptocurrency
- Ethereum
---
