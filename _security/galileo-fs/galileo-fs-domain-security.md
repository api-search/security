---
api_specs:
- filename: galileo-fs-config-api-openapi.yml
  format: yaml
  label: Galileo Financial Technologies Config API
  slug: galileo-fs-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galileo-fs/refs/heads/main/openapi/galileo-fs-config-api-openapi.yml
- filename: galileo-fs-dispute-api-openapi.yml
  format: yaml
  label: Galileo Financial Technologies Dispute API
  slug: galileo-fs-dispute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galileo-fs/refs/heads/main/openapi/galileo-fs-dispute-api-openapi.yml
- filename: galileo-fs-events-api-openapi.yml
  format: yaml
  label: Galileo Financial Technologies Events API
  slug: galileo-fs-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galileo-fs/refs/heads/main/openapi/galileo-fs-events-api-openapi.yml
- filename: galileo-fs-externaltransactions-api-openapi.yml
  format: yaml
  label: Galileo Financial Technologies ExternalTransactions API
  slug: galileo-fs-externaltransactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galileo-fs/refs/heads/main/openapi/galileo-fs-externaltransactions-api-openapi.yml
- filename: galileo-fs-loan-api-openapi.yml
  format: yaml
  label: Galileo Financial Technologies Loan API
  slug: galileo-fs-loan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galileo-fs/refs/heads/main/openapi/galileo-fs-loan-api-openapi.yml
- filename: galileo-fs-paymenthub-api-openapi.yml
  format: yaml
  label: Galileo Financial Technologies PaymentHub API
  slug: galileo-fs-paymenthub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galileo-fs/refs/heads/main/openapi/galileo-fs-paymenthub-api-openapi.yml
- filename: galileo-fs-program-api-openapi.yml
  format: yaml
  label: Galileo Financial Technologies Program API
  slug: galileo-fs-program-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galileo-fs/refs/heads/main/openapi/galileo-fs-program-api-openapi.yml
- filename: galileo-fs-risk-api-openapi.yml
  format: yaml
  label: Galileo Financial Technologies Risk API
  slug: galileo-fs-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galileo-fs/refs/heads/main/openapi/galileo-fs-risk-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: galileo-ft.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gpsrv.com
  spf: true
hosts:
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: www.galileo-ft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 11:15:34 2026 GMT
  host: docs.galileo-ft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 10:40:29 2026 GMT
  host: api-sandbox.cv.gpsrv.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Galileo Fs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Galileo Financial Technologies, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Galileo Financial Technologies
provider_slug: galileo-fs
slug: galileo-fs-domain-security
source_filename: galileo-fs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.galileo-ft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: false\n- host: docs.galileo-ft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 11:15:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-sandbox.cv.gpsrv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 10:40:29 2026 GMT\n  hsts: null\ndomains:\n- domain: galileo-ft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: gpsrv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/galileo-fs/refs/heads/main/security/galileo-fs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- BaaS
- Card Issuing
- Banking
- Payments
- ACH
---
