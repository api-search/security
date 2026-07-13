---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rapyd.net
  spf: true
hosts:
- cert_expires: Aug 25 16:48:35 2026 GMT
  host: www.rapyd.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 23:59:59 2026 GMT
  host: docs.rapyd.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 08:13:22 2026 GMT
  host: api.rapyd.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rapyd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rapyd, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rapyd
provider_slug: rapyd
slug: rapyd-domain-security
source_filename: rapyd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rapyd.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 16:48:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.rapyd.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 23:59:59 2026 GMT\n  hsts: false\n- host: api.rapyd.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 08:13:22 2026 GMT\n  hsts: null\ndomains:\n- domain: rapyd.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapyd/refs/heads/main/security/rapyd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Payments
- Cross-Border
- Cards
- Wallets
---
