---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: useorigin.com
  spf: true
hosts:
- cert_expires: Sep 30 03:16:40 2026 GMT
  host: useorigin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blend Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blend Financial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blend Financial
provider_slug: blend-financial
slug: blend-financial-domain-security
source_filename: blend-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: useorigin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 03:16:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: useorigin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blend-financial/refs/heads/main/security/blend-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Personal Finance
- Wealth Management
- Budgeting
- Investing
- Fintech
- Financial Planning
---
