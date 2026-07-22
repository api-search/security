---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vauld.com
  spf: true
hosts:
- cert_expires: Oct  3 17:31:22 2026 GMT
  host: www.vauld.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 17:31:22 2026 GMT
  host: docs.vauld.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 17:31:22 2026 GMT
  host: api.vauld.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vauld Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vauld, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vauld
provider_slug: vauld
slug: vauld-domain-security
source_filename: vauld-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vauld.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 17:31:22 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: docs.vauld.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 17:31:22 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api.vauld.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 17:31:22 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: vauld.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vauld/refs/heads/main/security/vauld-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Lending
- Borrowing
- Trading
- Wallets
- KYC
- Fintech
- India
- Singapore
---
