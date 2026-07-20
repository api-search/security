---
api_specs:
- filename: bitski-nft-service-openapi-original.json
  format: json
  label: Bitski NFT Service APIs
  slug: bitski-nft-service-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitski/refs/heads/main/openapi/bitski-nft-service-openapi-original.json
- filename: bitski-wallet-experience-openapi-original.json
  format: json
  label: Bitski Wallet Experience APIs
  slug: bitski-wallet-experience-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitski/refs/heads/main/openapi/bitski-wallet-experience-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bitski.com
  spf: true
hosts:
- cert_expires: Sep 25 16:44:13 2026 GMT
  host: bitski.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitski Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitski, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bitski
provider_slug: bitski
slug: bitski-domain-security
source_filename: bitski-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitski.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 16:44:13 2026 GMT\n  hsts: null\ndomains:\n- domain: bitski.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitski/refs/heads/main/security/bitski-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Web3
- Crypto Wallet
- Wallet as a Service
- NFT
- Blockchain
- Authentication
- OAuth
- Payments
- Developer Tools
- Company
---
