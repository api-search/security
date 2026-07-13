---
api_specs:
- filename: docs
  format: yaml
  label: Zora Coins SDK REST API
  slug: coins-rest-api
  spec_type: OpenAPI
  url: https://api-sdk.zora.engineering/docs
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: zora.co
  spf: true
hosts:
- cert_expires: Oct  9 15:15:11 2026 GMT
  host: zora.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 15:15:11 2026 GMT
  host: api.zora.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 16:37:33 2026 GMT
  host: docs.zora.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zora, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Zora
provider_slug: zora
slug: zora-domain-security
source_filename: zora-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zora.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 15:15:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.zora.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 15:15:11 2026 GMT\n  hsts: null\n- host: docs.zora.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 16:37:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: zora.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zora/refs/heads/main/security/zora-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- NFT
- Web3
- Blockchain
- Ethereum
- L2
- Creator Economy
- Marketplace
- Zora Network
- Base
- Optimism
---
