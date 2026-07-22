---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getapron.com
  spf: true
hosts:
- cert_expires: Aug 29 04:02:49 2026 GMT
  host: getapron.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apron Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apron, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apron
provider_slug: apron
slug: apron-domain-security
source_filename: apron-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getapron.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 04:02:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: getapron.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apron/refs/heads/main/security/apron-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Accounts Payable
- Bill Pay
- Accounting
- Payroll
- Expenses
- SMB
- Reconciliation
---
