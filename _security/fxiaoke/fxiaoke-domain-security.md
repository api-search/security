---
description: ''
domains:
- caa:
  - 1663594555720867329.zga.globalconnetct.com.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: fxiaoke.com
  spf: true
hosts:
- cert_expires: Nov  1 02:36:03 2026 GMT
  host: www.fxiaoke.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 02:36:03 2026 GMT
  host: developer.fxiaoke.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 02:36:03 2026 GMT
  host: open.fxiaoke.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Fxiaoke Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fxiaoke, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Fxiaoke
provider_slug: fxiaoke
slug: fxiaoke-domain-security
source_filename: fxiaoke-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fxiaoke.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 02:36:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.fxiaoke.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 02:36:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: open.fxiaoke.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  1 02:36:03 2026 GMT\n  hsts: false\ndomains:\n- domain: fxiaoke.com\n  dnssec: true\n  caa:\n  - 1663594555720867329.zga.globalconnetct.com.\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fxiaoke/refs/heads/main/security/fxiaoke-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise
- CRM
- Sales
- Marketing
- Customer Service
- SaaS
- China
- PaaS
---
