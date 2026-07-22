---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: doinstruct.com
  spf: true
hosts:
- cert_expires: Oct 14 04:26:13 2026 GMT
  host: www.doinstruct.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Doinstruct Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for doinstruct, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: doinstruct
provider_slug: doinstruct
slug: doinstruct-domain-security
source_filename: doinstruct-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.doinstruct.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 04:26:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: doinstruct.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doinstruct/refs/heads/main/security/doinstruct-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SaaS
- Training
- Compliance
- Frontline
- Learning
- Workforce
- Safety
- Artificial Intelligence
---
