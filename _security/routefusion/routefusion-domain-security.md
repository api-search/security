---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: routefusion.com
  spf: true
hosts:
- cert_expires: Aug 22 09:56:18 2026 GMT
  host: routefusion.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 11:47:13 2026 GMT
  host: docs.routefusion.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 14:55:13 2026 GMT
  host: external.routefusion.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Routefusion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Routefusion, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Routefusion
provider_slug: routefusion
slug: routefusion-domain-security
source_filename: routefusion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: routefusion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 09:56:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.routefusion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 11:47:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: external.routefusion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 14:55:13 2026 GMT\n  hsts: null\ndomains:\n- domain: routefusion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/routefusion/refs/heads/main/security/routefusion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Cross-Border Payments
- Global Payments
- FX
- Wallets
- GraphQL
- Stablecoin
---
