---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bygravity.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: runorion.com
  spf: true
hosts:
- cert_expires: Oct 10 11:55:32 2026 GMT
  host: www.bygravity.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 19:59:31 2026 GMT
  host: docs.runorion.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 03:09:54 2026 GMT
  host: g.runorion.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orion By Gravity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orion by Gravity, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Orion by Gravity
provider_slug: orion-by-gravity
slug: orion-by-gravity-domain-security
source_filename: orion-by-gravity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bygravity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 11:55:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.runorion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 19:59:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: g.runorion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 03:09:54 2026 GMT\n  hsts: null\ndomains:\n- domain: bygravity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: runorion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orion-by-gravity/refs/heads/main/security/orion-by-gravity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Analytics
- Business Intelligence
- Artificial Intelligence
- Data
- MCP
- Data Warehouse
- SaaS
---
