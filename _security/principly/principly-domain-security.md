---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: backer.com
  spf: true
hosts:
- cert_expires: Aug 21 04:50:04 2026 GMT
  host: backer.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Principly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Principly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Principly
provider_slug: principly
slug: principly-domain-security
source_filename: principly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: backer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 04:50:04 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: backer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/principly/refs/heads/main/security/principly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Financial Services
- 529 Plans
- Education Savings
- College Savings
- Consumer Finance
- Investment Adviser
- Mobile App
---
