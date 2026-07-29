---
api_specs:
- filename: helius-asyncapi.yml
  format: yaml
  label: Helius Solana RPC
  slug: rpc
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/asyncapi/helius-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: helius.dev
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: helius.xyz
  spf: true
hosts:
- cert_expires: Sep  4 07:05:23 2026 GMT
  host: www.helius.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 09:05:41 2026 GMT
  host: api.helius.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 01:59:43 2026 GMT
  host: laserstream-mainnet.helius-rpc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Helius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Helius, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: Helius
provider_slug: helius
slug: helius-domain-security
source_filename: helius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.helius.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 07:05:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.helius.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 09:05:41 2026 GMT\n  hsts: null\n- host: laserstream-mainnet.helius-rpc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 01:59:43 2026 GMT\n  hsts: false\ndomains:\n- domain: helius.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: helius.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/security/helius-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Web3
- Blockchain
- Solana
- RPC
- DAS
- Streams
---
