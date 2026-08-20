---
api_specs:
- filename: truist-financial-accounts-api-openapi.yml
  format: yaml
  label: Truist Financial Accounts API
  slug: truist-financial-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truist-financial/refs/heads/main/openapi/truist-financial-accounts-api-openapi.yml
- filename: truist-financial-commercial-accounts-api-openapi.yml
  format: yaml
  label: Truist Financial Commercial Accounts API
  slug: truist-financial-commercial-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truist-financial/refs/heads/main/openapi/truist-financial-commercial-accounts-api-openapi.yml
- filename: truist-financial-commercial-transactions-api-openapi.yml
  format: yaml
  label: Truist Financial Commercial Transactions API
  slug: truist-financial-commercial-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truist-financial/refs/heads/main/openapi/truist-financial-commercial-transactions-api-openapi.yml
- filename: truist-financial-transactions-api-openapi.yml
  format: yaml
  label: Truist Financial Transactions API
  slug: truist-financial-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truist-financial/refs/heads/main/openapi/truist-financial-transactions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "ccs_certificate_services@truist.com"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: truist.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: site.com
  spf: true
hosts:
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: www.truist.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: developer.truist.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: truist-1132.my.site.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Truist Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Truist Financial, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Truist Financial
provider_slug: truist-financial
slug: truist-financial-domain-security
source_filename: truist-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.truist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.truist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: null\n- host: truist-1132.my.site.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: truist.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"ccs_certificate_services@truist.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: site.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truist-financial/refs/heads/main/security/truist-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Banking
- Financial-Services
- Open Banking
- Commercial Banking
- Personal Banking
- Payments
- Account
- Transaction
- Fortune 500
---
