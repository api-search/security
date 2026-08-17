---
api_specs:
- filename: deluxe-dpp-gateway-openapi.yml
  format: yaml
  label: Deluxe Payments Platform — Gateway Experience API
  slug: deluxe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-dpp-gateway-openapi.yml
- filename: deluxe-dpp-reports-openapi.yml
  format: yaml
  label: Deluxe Payments Platform — Reports Experience API
  slug: dpp-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-dpp-reports-openapi.yml
- filename: deluxe-dpp-invoices-openapi.yml
  format: yaml
  label: Deluxe Payments Platform — Invoice Experience API
  slug: dpp-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-dpp-invoices-openapi.yml
- filename: deluxe-postman-sandbox-openapi.yml
  format: yaml
  label: Deluxe Payments Platform — Sandbox API (Deluxe-published OpenAPI)
  slug: dpp-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-postman-sandbox-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: deluxe.com
  spf: false
hosts:
- cert_expires: Oct 26 04:41:06 2026 GMT
  host: www.deluxe.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 16:31:34 2026 GMT
  host: developer.deluxe.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 18:46:19 2026 GMT
  host: api.deluxe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deluxe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deluxe Corporation, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Deluxe Corporation
provider_slug: deluxe
slug: deluxe-domain-security
source_filename: deluxe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deluxe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 04:41:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.deluxe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 16:31:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.deluxe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 18:46:19 2026 GMT\n  hsts: null\ndomains:\n- domain: deluxe.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/security/deluxe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Merchant Services
- Card Processing
- ACH
- Invoicing
- Subscriptions
- Tokenization
- Webhooks
- Reporting
- Data Analytics
- Marketing
- Small Business
---
