---
api_specs:
- filename: docs
  format: yaml
  label: Frax Finance Combined Data API
  slug: frax-finance-combined-data-api
  spec_type: OpenAPI
  url: https://api.frax.finance/v1/docs
- filename: docs
  format: yaml
  label: Frax Finance Pools API
  slug: frax-finance-pools-api
  spec_type: OpenAPI
  url: https://api.frax.finance/v1/docs
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: frax.finance
  spf: true
hosts:
- cert_expires: Sep 10 21:20:46 2026 GMT
  host: frax.finance
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 14:16:52 2026 GMT
  host: docs.frax.finance
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 16:12:08 2026 GMT
  host: api.frax.finance
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Frax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Frax Finance, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Frax Finance
provider_slug: frax
slug: frax-domain-security
source_filename: frax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: frax.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 21:20:46 2026 GMT\n  hsts: false\n- host: docs.frax.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 14:16:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.frax.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 16:12:08 2026 GMT\n  hsts: null\ndomains:\n- domain: frax.finance\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frax/refs/heads/main/security/frax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- DeFi
- Stablecoin
- Fractional-Algorithmic
- Ethereum
- frxETH
- Liquid Staking
- AMO
- Collateral
---
