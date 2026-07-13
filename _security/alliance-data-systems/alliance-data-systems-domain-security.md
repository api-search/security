---
api_specs:
- filename: bread-pay-platform-openapi.yml
  format: yaml
  label: Bread Pay Platform API
  slug: bread-pay-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alliance-data-systems/refs/heads/main/openapi/bread-pay-platform-openapi.yml
- filename: bread-classic-merchant-openapi.yml
  format: yaml
  label: Bread Classic Merchant API
  slug: bread-classic-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alliance-data-systems/refs/heads/main/openapi/bread-classic-merchant-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: breadfinancial.com
  spf: true
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: breadpayments.com
  spf: true
hosts:
- cert_expires: Aug 26 21:51:58 2026 GMT
  host: www.breadfinancial.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 13:09:15 2026 GMT
  host: platform-docs.breadpayments.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 21:51:58 2026 GMT
  host: api.platform.breadpayments.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alliance Data Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alliance Data Systems (Bread Financial Holdings), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alliance Data Systems (Bread Financial Holdings)
provider_slug: alliance-data-systems
slug: alliance-data-systems-domain-security
source_filename: alliance-data-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.breadfinancial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 21:51:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform-docs.breadpayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 13:09:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.platform.breadpayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 21:51:58 2026 GMT\n  hsts: null\ndomains:\n- domain: breadfinancial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: breadpayments.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alliance-data-systems/refs/heads/main/security/alliance-data-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Fintech
- Buy Now Pay Later
- BNPL
- Bread Pay
- Private Label Credit
- Co Brand Credit Cards
- Loyalty Programs
- Marketing
- Data Driven Marketing
- Payments
- Lending
- Savings
- Personal Loans
- Consumer Banking
- Retail Finance
- Fortune 500
- NYSE BFH
- Comenity Bank
- Rebrand
---
