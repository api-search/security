---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: yourika.ai
  spf: false
hosts:
- cert_expires: Sep  6 23:11:37 2026 GMT
  host: yourika.ai
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yourika Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for YOURIKA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: YOURIKA
provider_slug: yourika
slug: yourika-domain-security
source_filename: yourika-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yourika.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:11:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: yourika.ai\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yourika/refs/heads/main/security/yourika-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Healthcare
- Nursing
- Workforce
- Long-term Care
- Venture Studio
- Education
---
