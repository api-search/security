---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: usegrade.com
  spf: true
hosts:
- cert_expires: Oct 15 00:15:24 2026 GMT
  host: usegrade.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Grade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grade, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Grade
provider_slug: grade
slug: grade-domain-security
source_filename: grade-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usegrade.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 00:15:24 2026 GMT\n  hsts: false\ndomains:\n- domain: usegrade.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grade/refs/heads/main/security/grade-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payroll
- Payments
- Payouts
- Compliance
- Creator Economy
- Fintech
- Contractors
- Merchant of Record
- API
---
