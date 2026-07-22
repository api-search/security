---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mujer-financiera.com
  spf: true
hosts:
- cert_expires: Oct  1 08:29:18 2026 GMT
  host: mujer-financiera.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mujer Financiera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mujer Financiera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mujer Financiera
provider_slug: mujer-financiera
slug: mujer-financiera-domain-security
source_filename: mujer-financiera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mujer-financiera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 08:29:18 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: mujer-financiera.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mujer-financiera/refs/heads/main/security/mujer-financiera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Education
- Fintech
- Edtech
- Personal Finance
- Investing
- Women
- Latin America
---
