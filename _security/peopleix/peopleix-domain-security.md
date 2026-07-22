---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: peopleix.com
  spf: true
hosts:
- cert_expires: Aug 24 05:40:28 2026 GMT
  host: www.peopleix.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Peopleix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Peopleix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Peopleix
provider_slug: peopleix
slug: peopleix-domain-security
source_filename: peopleix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.peopleix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 05:40:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: peopleix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peopleix/refs/heads/main/security/peopleix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- HR
- People Analytics
- People Intelligence
- Conversation Intelligence
- Human Resources
- Workforce Analytics
- AI
- MCP
- Germany
---
