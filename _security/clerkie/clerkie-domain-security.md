---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: clerkie.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: getfiber.ai
  spf: false
hosts:
- cert_expires: Oct  1 21:43:47 2026 GMT
  host: www.clerkie.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 13:14:22 2026 GMT
  host: www.getfiber.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: api.clerkie.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clerkie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clerkie, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Clerkie
provider_slug: clerkie
slug: clerkie-domain-security
source_filename: clerkie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clerkie.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 21:43:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.getfiber.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 13:14:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.clerkie.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: clerkie.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: getfiber.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clerkie/refs/heads/main/security/clerkie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Debt Management
- Lending
- Loan Servicing
- Debt Collection
- Payments
- Credit
- Financial-Services
- Personal Finance
- AI Agent
- Consumer Finance
---
