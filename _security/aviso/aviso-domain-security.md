---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aviso.com
  spf: true
hosts:
- cert_expires: Aug 29 17:55:22 2026 GMT
  host: www.aviso.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aviso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aviso, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aviso
provider_slug: aviso
slug: aviso-domain-security
source_filename: aviso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aviso.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 17:55:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aviso.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aviso/refs/heads/main/security/aviso-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Revenue Intelligence
- Sales
- Artificial Intelligence
- Forecasting
- Conversation Intelligence
- RevOps
- Analytics
---
