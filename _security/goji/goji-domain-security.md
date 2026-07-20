---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: goji.investments
  spf: true
hosts:
- cert_expires: Aug 29 16:38:33 2026 GMT
  host: goji.investments
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 18:36:35 2026 GMT
  host: docs.api.goji.investments
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: api.goji.investments
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Goji Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Goji, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Goji
provider_slug: goji
slug: goji-domain-security
source_filename: goji-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goji.investments\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 16:38:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.api.goji.investments\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 18:36:35 2026 GMT\n  hsts: false\n- host: api.goji.investments\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: goji.investments\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goji/refs/heads/main/security/goji-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Private Markets
- Investments
- Funds
- KYC
- Payments
- ISA
- Settlement
- Webhooks
- Euroclear
---
