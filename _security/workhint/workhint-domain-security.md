---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: workhint.com
  spf: true
hosts:
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: workhint.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workhint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workhint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Workhint
provider_slug: workhint
slug: workhint-domain-security
source_filename: workhint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: workhint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: workhint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workhint/refs/heads/main/security/workhint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Workforce Management
- Work Orchestration
- Staffing
- Payments
- Contract Management
- Compliance
- Artificial Intelligence
- SaaS
---
