---
api_specs:
- filename: memeswap-fun-research-api-openapi.yml
  format: yaml
  label: MemeSwap Research API
  slug: memeswap-fun-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memeswap-fun/openapi/memeswap-fun-research-api-openapi.yml
- filename: memeswap-fun-routing-api-openapi.yml
  format: yaml
  label: MemeSwap Routing API
  slug: memeswap-fun-routing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memeswap-fun/openapi/memeswap-fun-routing-api-openapi.yml
- filename: memeswap-fun-solana-rpc-api-openapi.yml
  format: yaml
  label: MemeSwap Solana RPC API
  slug: memeswap-fun-solana-rpc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memeswap-fun/openapi/memeswap-fun-solana-rpc-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: memeswap.fun
  spf: true
hosts:
- cert_expires: Jan 25 16:00:01 2027 GMT
  host: memeswap.fun
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MemeSwap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MemeSwap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: MemeSwap
provider_slug: memeswap-fun
slug: memeswap-fun-domain-security
source_filename: memeswap-fun-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memeswap.fun\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 16:00:01 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: memeswap.fun\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/memeswap-fun/security/memeswap-fun-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cryptocurrency
- Meme Coins
- Swap
- Bridge
- Non-Custodial
- iPhone App
---
