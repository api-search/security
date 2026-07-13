---
api_specs:
- filename: zerodev-openapi.yml
  format: yaml
  label: ZeroDev Bundler RPC
  slug: zerodev-bundler-rpc
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerodev/refs/heads/main/openapi/zerodev-openapi.yml
- filename: zerodev-openapi.yml
  format: yaml
  label: ZeroDev Paymaster RPC
  slug: zerodev-paymaster-rpc
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerodev/refs/heads/main/openapi/zerodev-openapi.yml
- filename: zerodev-openapi.yml
  format: yaml
  label: ZeroDev Kernel SDK
  slug: zerodev-kernel-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerodev/refs/heads/main/openapi/zerodev-openapi.yml
- filename: zerodev-openapi.yml
  format: yaml
  label: ZeroDev Meta-Aggregator (Smart Routing)
  slug: zerodev-meta-aggregator
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerodev/refs/heads/main/openapi/zerodev-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: zerodev.app
  spf: true
hosts:
- cert_expires: Oct  5 15:30:48 2026 GMT
  host: zerodev.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 19:54:00 2026 GMT
  host: docs.zerodev.app
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 04:07:02 2026 GMT
  host: rpc.zerodev.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zerodev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZeroDev, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: ZeroDev
provider_slug: zerodev
slug: zerodev-domain-security
source_filename: zerodev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zerodev.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 15:30:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.zerodev.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 19:54:00 2026 GMT\n  hsts: false\n- host: rpc.zerodev.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 04:07:02 2026 GMT\n  hsts: null\ndomains:\n- domain: zerodev.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zerodev/refs/heads/main/security/zerodev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Account Abstraction
- Smart Wallets
- ERC-4337
- EIP-7702
- Paymaster
- Bundler
- JSON-RPC
- Web3
---
