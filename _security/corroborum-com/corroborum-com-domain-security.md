---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: corroborum.com
  spf: true
hosts:
- cert_expires: Jan 15 14:15:16 2027 GMT
  host: corroborum.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Corroborum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corroborum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Corroborum
provider_slug: corroborum-com
slug: corroborum-com-domain-security
source_filename: corroborum-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corroborum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 14:15:16 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: corroborum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/corroborum-com/security/corroborum-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Academic Research
- Literature Search
- Scholarly Papers
- MCP
- AI Assistant
- Citations
---
