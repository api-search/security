---
api_specs:
- filename: scalapay-instore-api-openapi.yml
  format: yaml
  label: Scalapay Instore API
  slug: scalapay-instore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalapay/refs/heads/main/openapi/scalapay-instore-api-openapi.yml
- filename: scalapay-orders-api-openapi.yml
  format: yaml
  label: Scalapay Orders API
  slug: scalapay-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalapay/refs/heads/main/openapi/scalapay-orders-api-openapi.yml
- filename: scalapay-reporting-api-openapi.yml
  format: yaml
  label: Scalapay Reporting API
  slug: scalapay-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalapay/refs/heads/main/openapi/scalapay-reporting-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: scalapay.com
  spf: true
hosts:
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: www.scalapay.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: integration.api.scalapay.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: api.scalapay.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scalapay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scalapay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Scalapay
provider_slug: scalapay
slug: scalapay-domain-security
source_filename: scalapay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scalapay.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: false\n- host: integration.api.scalapay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.scalapay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: scalapay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalapay/refs/heads/main/security/scalapay-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Payments
- Buy Now Pay Later
- BNPL
- Instalments
- E-Commerce
- Checkout
- Financial Services
- Point of Sale
- Reconciliation
- Europe
- Company
---
