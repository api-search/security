---
api_specs:
- filename: ajaib-market-info-api-openapi.yml
  format: yaml
  label: Ajaib Market Info API
  slug: ajaib-market-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ajaib/refs/heads/main/openapi/ajaib-market-info-api-openapi.yml
- filename: ajaib-spot-trading-api-openapi.yml
  format: yaml
  label: Ajaib Spot Trading API
  slug: ajaib-spot-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ajaib/refs/heads/main/openapi/ajaib-spot-trading-api-openapi.yml
- filename: ajaib-wallet-api-openapi.yml
  format: yaml
  label: Ajaib Wallet API
  slug: ajaib-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ajaib/refs/heads/main/openapi/ajaib-wallet-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ajaib.co.id
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gitbook.io
  spf: true
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: ajaib.co.id
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: 'HSTS is served but the automated probe recorded null because the origin answers an unattended client with a Cloudflare 403 bot challenge. Confirmed by a browser-UA HEAD on 2026-08-06: strict-transport-security: max-age=31536000'
  tls_version: TLSv1.3
- cert_expires: Oct 15 19:03:12 2026 GMT
  host: ajaib.gitbook.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: api.ajaib.co.id
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: 'Same as ajaib.co.id: HSTS confirmed by browser-UA HEAD on 2026-08-06; the host is behind a Cloudflare bot challenge (403 on every path).'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ajaib Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ajaib, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Ajaib
provider_slug: ajaib
slug: ajaib-domain-security
source_filename: ajaib-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ajaib.co.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: >-\n    HSTS is served but the automated probe recorded null because the origin\n    answers an unattended client with a Cloudflare 403 bot challenge. Confirmed\n    by a browser-UA HEAD on 2026-08-06: strict-transport-security: max-age=31536000\n- host: ajaib.gitbook.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 19:03:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ajaib.co.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: >-\n    Same as ajaib.co.id: HSTS confirmed by browser-UA HEAD on 2026-08-06; the\n    host is behind a Cloudflare bot challenge (403 on every path).\ndomains:\n- domain: ajaib.co.id\n\
  \  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: gitbook.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nx-notes:\n  - >-\n    gitbook.io is GitBook's shared documentation host, not a domain Ajaib\n    controls; its DNSSEC/SPF/DMARC values describe GitBook, not Ajaib.\n  - >-\n    ajaib.co.id publishes DMARC with p=none, which requests no enforcement\n    action on failing mail. For a licensed brokerage this is the weakest of the\n    three DMARC policies.\n  - No CAA records are published for ajaib.co.id.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ajaib/refs/heads/main/security/ajaib-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Financial Services
- Investing
- Brokerage
- Trading
- Cryptocurrency
- Crypto Exchange
- Stocks
- Mutual Funds
- Fintech
- Indonesia
- Wealth Management
---
