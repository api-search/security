---
api_specs:
- filename: blowfish-v20230308-openapi-original.yml
  format: yaml
  label: Blowfish Scan API
  slug: blowfish-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blowfish/refs/heads/main/openapi/blowfish-v20230308-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: blowfish.xyz
  spf: true
hosts:
- cert_expires: Aug 23 19:47:27 2026 GMT
  host: blowfish.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: free.api.blowfish.xyz
  https: false
- cert_expires: Aug 23 19:47:27 2026 GMT
  host: api.blowfish.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blowfish Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blowfish, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Blowfish
provider_slug: blowfish
slug: blowfish-domain-security
source_filename: blowfish-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blowfish.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 19:47:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: free.api.blowfish.xyz\n  https: false\n- host: api.blowfish.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 19:47:27 2026 GMT\n  hsts: null\ndomains:\n- domain: blowfish.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blowfish/refs/heads/main/security/blowfish-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Web3
- Blockchain
- Wallet
- Transaction Scanning
- Fraud Prevention
- Cryptocurrency
---
