---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getclair.com
  spf: true
hosts:
- cert_expires: Oct 12 11:02:31 2026 GMT
  host: getclair.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clair Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clair, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clair
provider_slug: clair
slug: clair-domain-security
source_filename: clair-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getclair.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 11:02:31 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: getclair.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clair/refs/heads/main/security/clair-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial-Services
- Fintech
- Earned Wage Access
- On-Demand Pay
- Payroll
- Embedded Finance
- Banking
- Human Resources
---
