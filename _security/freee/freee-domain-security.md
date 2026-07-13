---
api_specs:
- filename: freee-openapi.yml
  format: yaml
  label: freee Accounting Deals API
  slug: freee-accounting-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee Accounting Account Items API
  slug: freee-accounting-account-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee Accounting Partners API
  slug: freee-accounting-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee Accounting Invoices and Quotations API
  slug: freee-accounting-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee Accounting Wallet Transactions API
  slug: freee-accounting-wallet-txns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee Accounting Journals and Reports API
  slug: freee-accounting-journals-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee HR Employees API
  slug: freee-hr-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee HR Payroll API
  slug: freee-hr-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee HR Attendance API
  slug: freee-hr-attendance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_pct: 100
  dmarc_policy: quarantine
  dmarc_rua: mailto:psirt@freee.co.jp
  dnssec: false
  domain: freee.co.jp
  spf: true
  spf_policy: ~all (softfail); includes _spf.google.com, amazonses.com, mktomail.com, salesforce/pardot, hubspot
hosts:
- cert_expires: Mar 20 05:19:20 2027 GMT
  cert_issuer: GlobalSign nv-sa (GlobalSign GCC R6 AlphaSSL CA 2025)
  host: www.freee.co.jp
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  cert_issuer: Amazon (Amazon RSA 2048 M04)
  host: api.freee.co.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  7 23:59:59 2027 GMT
  cert_issuer: Amazon (Amazon RSA 2048 M04)
  host: accounts.secure.freee.co.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.freee.co.jp
  hsts: false
  https: true
  note: Developer documentation portal; HTTPS reachable, HSTS header not observed.
kind: domain-security
layout: security
method: probed
name: Freee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for freee, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: freee
provider_slug: freee
slug: freee-domain-security
source_filename: freee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.freee.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: GlobalSign nv-sa (GlobalSign GCC R6 AlphaSSL CA 2025)\n  cert_expires: Mar 20 05:19:20 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api.freee.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Amazon (Amazon RSA 2048 M04)\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: false\n- host: accounts.secure.freee.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Amazon (Amazon RSA 2048 M04)\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: false\n- host: developer.freee.co.jp\n  https: true\n  hsts: false\n  note: Developer documentation portal; HTTPS reachable, HSTS header not observed.\ndomains:\n- domain: freee.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: \"~all (softfail); includes _spf.google.com, amazonses.com, mktomail.com, salesforce/pardot,\
  \ hubspot\"\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_pct: 100\n  dmarc_rua: mailto:psirt@freee.co.jp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/security/freee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- Bookkeeping
- HR
- Payroll
- Invoicing
- Finance
- SaaS
- Japan
---
