---
api_specs:
- filename: bill-webhooks-asyncapi.yml
  format: yaml
  label: BILL v3 API
  slug: v3-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bill/refs/heads/main/asyncapi/bill-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bill.com
  spf: true
hosts:
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: www.bill.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 04:23:26 2026 GMT
  host: developer.bill.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: gateway.prod.bill.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BILL, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BILL
provider_slug: bill
slug: bill-domain-security
source_filename: bill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.bill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 04:23:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gateway.prod.bill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bill.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bill/refs/heads/main/security/bill-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounts Payable
- Accounts Receivable
- Spend Management
- Expense Management
- Payments
- Bill Pay
- Financial Operations
- Fintech
---
