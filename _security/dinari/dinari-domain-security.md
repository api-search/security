---
api_specs:
- filename: dinari-openapi-original.yml
  format: yaml
  label: Dinari Enterprise API
  slug: dinari-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/openapi/dinari-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dinari.com
  spf: true
hosts:
- cert_expires: Oct 14 21:51:25 2026 GMT
  host: dinari.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 01:39:23 2026 GMT
  host: api-enterprise.sbt.dinari.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dinari Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dinari, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dinari
provider_slug: dinari
slug: dinari-domain-security
source_filename: dinari-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dinari.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 21:51:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-enterprise.sbt.dinari.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 01:39:23 2026 GMT\n  hsts: null\ndomains:\n- domain: dinari.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/security/dinari-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Tokenized Securities
- Stocks
- ETFs
- Brokerage
- Market Data
- Blockchain
- Stablecoin
- Fintech
- KYC
- Orders
- Wallets
---
