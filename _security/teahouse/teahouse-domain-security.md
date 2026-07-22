---
api_specs:
- filename: teahouse-vault-openapi.yml
  format: yaml
  label: Teahouse Vault API
  slug: teahouse-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teahouse/refs/heads/main/openapi/teahouse-vault-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: teahouse.finance
  spf: true
hosts:
- cert_expires: Aug 27 08:01:09 2026 GMT
  host: teahouse.finance
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teahouse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teahouse Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Teahouse Finance
provider_slug: teahouse
slug: teahouse-domain-security
source_filename: teahouse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: teahouse.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 08:01:09 2026 GMT\n  hsts: false\ndomains:\n- domain: teahouse.finance\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teahouse/refs/heads/main/security/teahouse-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Crypto
- DeFi
- Blockchain
- Vaults
- Liquidity Management
- Asset Management
- Uniswap
- Web3
---
