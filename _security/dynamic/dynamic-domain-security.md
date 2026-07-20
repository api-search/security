---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dynamic.xyz
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dynamicauth.com
  spf: true
hosts:
- cert_expires: Oct 12 17:19:58 2026 GMT
  host: www.dynamic.xyz
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 21:16:47 2026 GMT
  host: app.dynamicauth.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dynamic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dynamic, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Dynamic
provider_slug: dynamic
slug: dynamic-domain-security
source_filename: dynamic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dynamic.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 17:19:58 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: app.dynamicauth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 21:16:47 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: dynamic.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dynamicauth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dynamic/refs/heads/main/security/dynamic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Wallet Infrastructure
- Web3
- Crypto
- Authentication
- Embedded Wallets
- Stablecoins
- Key Management
- MPC
- Developer Tools
- Fintech
- Blockchain
---
