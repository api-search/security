---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: joinassembly.com
  spf: true
hosts:
- cert_expires: Oct  7 18:26:38 2026 GMT
  host: www.joinassembly.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Assembly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Assembly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Assembly
provider_slug: assembly
slug: assembly-domain-security
source_filename: assembly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.joinassembly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 18:26:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: joinassembly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/assembly/refs/heads/main/security/assembly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Developer Tools
- Employee Recognition
- Employee Engagement
- Rewards
- Human Resources
- Workplace
- SaaS
- Integrations
---
