---
api_specs:
- filename: datanomik-accounts-api-openapi.yml
  format: yaml
  label: Datanomik Accounts API
  slug: datanomik-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-accounts-api-openapi.yml
- filename: datanomik-applications-api-openapi.yml
  format: yaml
  label: Datanomik Applications API
  slug: datanomik-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-applications-api-openapi.yml
- filename: datanomik-balances-api-openapi.yml
  format: yaml
  label: Datanomik Balances API
  slug: datanomik-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-balances-api-openapi.yml
- filename: datanomik-general-owners-api-openapi.yml
  format: yaml
  label: Datanomik General Owners API
  slug: datanomik-general-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-general-owners-api-openapi.yml
- filename: datanomik-investments-api-openapi.yml
  format: yaml
  label: Datanomik Investments API
  slug: datanomik-investments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-investments-api-openapi.yml
- filename: datanomik-links-api-openapi.yml
  format: yaml
  label: Datanomik Links API
  slug: datanomik-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-links-api-openapi.yml
- filename: datanomik-payment-slips-api-openapi.yml
  format: yaml
  label: Datanomik Payment Slips API
  slug: datanomik-payment-slips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-payment-slips-api-openapi.yml
- filename: datanomik-payments-api-openapi.yml
  format: yaml
  label: Datanomik Payments API
  slug: datanomik-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-payments-api-openapi.yml
- filename: datanomik-pix-transactions-api-openapi.yml
  format: yaml
  label: Datanomik Pix Transactions API
  slug: datanomik-pix-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-pix-transactions-api-openapi.yml
- filename: datanomik-transactions-api-openapi.yml
  format: yaml
  label: Datanomik Transactions API
  slug: datanomik-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: datanomik.com
  spf: true
hosts:
- cert_expires: Sep 20 04:08:43 2026 GMT
  host: datanomik.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 16:15:43 2026 GMT
  host: docs.datanomik.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr 10 23:59:59 2027 GMT
  host: api.datanomik.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datanomik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datanomik, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Datanomik
provider_slug: datanomik
slug: datanomik-domain-security
source_filename: datanomik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datanomik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 04:08:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.datanomik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 16:15:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.datanomik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: datanomik.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/security/datanomik-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Open Finance
- Open Banking
- Treasury Management
- Cash Management
- Payments
- PIX
- Financial Data
- Bank Connectivity
- Brazil
- LatAm
- Fintech
---
