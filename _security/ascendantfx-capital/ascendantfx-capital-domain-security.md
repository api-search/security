---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ascendant.world
  spf: true
hosts:
- cert_expires: Aug 28 19:39:58 2026 GMT
  host: www.ascendant.world
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 12:44:16 2026 GMT
  host: api.ascendant.world
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ascendantfx Capital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AscendantFX Capital, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AscendantFX Capital
provider_slug: ascendantfx-capital
slug: ascendantfx-capital-domain-security
source_filename: ascendantfx-capital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ascendant.world\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 19:39:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ascendant.world\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 12:44:16 2026 GMT\n  hsts: null\ndomains:\n- domain: ascendant.world\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ascendantfx-capital/refs/heads/main/security/ascendantfx-capital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Cross-Border Payments
- Foreign Exchange
- FX
- International Payments
- B2B Payments
- Financial Services
- Fintech
---
