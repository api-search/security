---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: yield.xyz
  spf: false
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: yield.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 19:57:12 2026 GMT
  host: docs.yield.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: api.yield.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yieldxyz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yield.xyz, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Yield.xyz
provider_slug: yieldxyz
slug: yieldxyz-domain-security
source_filename: yieldxyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yield.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: false\n- host: docs.yield.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 19:57:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.yield.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: yield.xyz\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yieldxyz/refs/heads/main/security/yieldxyz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto Web3
- Staking
- DeFi
- Yield
- Blockchain
- Restaking
- Vaults
- Web3 Infrastructure
- Non-Custodial
---
