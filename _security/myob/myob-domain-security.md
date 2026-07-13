---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: myob.com
  spf: true
hosts:
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: www.myob.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 04:41:38 2026 GMT
  host: developer.myob.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 10:21:52 2026 GMT
  host: api.myob.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Myob Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MYOB, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MYOB
provider_slug: myob
slug: myob-domain-security
source_filename: myob-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.myob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.myob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 04:41:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.myob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 10:21:52 2026 GMT\n  hsts: null\ndomains:\n- domain: myob.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/myob/refs/heads/main/security/myob-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- Business Management
- Invoices
- Bills
- Contacts
- Payroll
- Tax
- Financial Reporting
- SMB
- Australia
- New Zealand
---
