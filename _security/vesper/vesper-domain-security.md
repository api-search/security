---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Vesper Finance API
  slug: vesper-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesper/refs/heads/main/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vesper.finance
  spf: true
hosts:
- cert_expires: Sep 16 05:59:24 2026 GMT
  host: vesper.finance
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 16:32:19 2026 GMT
  host: docs.vesper.finance
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: api.vesper.finance
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Vesper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vesper Finance, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vesper Finance
provider_slug: vesper
slug: vesper-domain-security
source_filename: vesper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vesper.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 05:59:24 2026 GMT\n  hsts: false\n- host: docs.vesper.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 16:32:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.vesper.finance\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: vesper.finance\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vesper/refs/heads/main/security/vesper-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DeFi
- Yield Aggregator
- Liquidity Pools
- APY
- Staking
- VSP Token
- Ethereum
- Polygon
- Avalanche
- Optimism
---
