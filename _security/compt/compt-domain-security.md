---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: compt.io
  spf: true
hosts:
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: compt.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Compt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Compt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Compt
provider_slug: compt
slug: compt-domain-security
source_filename: compt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: compt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: compt.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/compt/refs/heads/main/security/compt-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Human Resources
- Employee Benefits
- Stipends
- Lifestyle Spending Account
- Reimbursement
- Payroll
- HR Tech
---
