---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nowpay.cash
  spf: true
hosts:
- cert_expires: Sep 25 04:53:39 2026 GMT
  host: nowpay.cash
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nowpay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nowpay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Nowpay
provider_slug: nowpay
slug: nowpay-domain-security
source_filename: nowpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nowpay.cash\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 04:53:39 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: nowpay.cash\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nowpay/refs/heads/main/security/nowpay-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Fintech
- Financial Wellness
- Earned Wage Access
- Salary Advance
- Payroll
- Employee Benefits
- Embedded Finance
- Payments
---
