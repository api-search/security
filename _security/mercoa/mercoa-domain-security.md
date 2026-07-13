---
api_specs:
- filename: mercoa-openapi.yml
  format: yaml
  label: Mercoa API
  slug: mercoa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercoa/refs/heads/main/openapi/mercoa-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mercoa.com
  spf: true
hosts:
- cert_expires: Oct  7 00:42:23 2026 GMT
  host: mercoa.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 05:29:52 2026 GMT
  host: docs.mercoa.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 00:42:23 2026 GMT
  host: api.mercoa.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mercoa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mercoa, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mercoa
provider_slug: mercoa
slug: mercoa-domain-security
source_filename: mercoa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mercoa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 00:42:23 2026 GMT\n  hsts: false\n- host: docs.mercoa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 05:29:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mercoa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 00:42:23 2026 GMT\n  hsts: null\ndomains:\n- domain: mercoa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercoa/refs/heads/main/security/mercoa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Mercoa
- Embedded Finance
- Accounts Payable
- Accounts Receivable
- BillPay
- Invoicing
- Payments
- Vertical SaaS
- Vendors
- Approvals
- Disbursements
- Virtual Cards
---
