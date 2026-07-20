---
api_specs:
- filename: babylon-labs-staking-api-openapi-original.yml
  format: yaml
  label: Babylon Staking API
  slug: babylon-staking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/openapi/babylon-labs-staking-api-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: babylonlabs.io
  spf: true
hosts:
- cert_expires: Aug 21 20:15:16 2026 GMT
  host: babylonlabs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Babylon Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Babylon Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Babylon Labs
provider_slug: babylon-labs
slug: babylon-labs-domain-security
source_filename: babylon-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: babylonlabs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 20:15:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: babylonlabs.io\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/security/babylon-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto Defi
- Bitcoin
- Bitcoin Staking
- Blockchain
- Cosmos
- Proof of Stake
- DeFi
- Staking
- API
---
