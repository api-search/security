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
- cert_expires: Aug 14 10:18:41 2026 GMT
  host: www.dynamic.xyz
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 01:46:08 2026 GMT
  host: docs.dynamic.xyz
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
name: Dynamic Xyz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dynamic, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Dynamic
provider_slug: dynamic-xyz
slug: dynamic-xyz-domain-security
source_filename: dynamic-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dynamic.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 10:18:41 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: docs.dynamic.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 01:46:08 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: app.dynamicauth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 21:16:47 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: dynamic.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dynamicauth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dynamic-xyz/refs/heads/main/security/dynamic-xyz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Web3
- Wallets
- Authentication
- Embedded Wallets
- MPC
---
