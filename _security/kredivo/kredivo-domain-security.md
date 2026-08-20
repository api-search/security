---
api_specs:
- filename: kredivo-calculator-api-openapi.yml
  format: yaml
  label: Kredivo Calculator API
  slug: kredivo-calculator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kredivo/refs/heads/main/openapi/kredivo-calculator-api-openapi.yml
- filename: kredivo-checkout-api-openapi.yml
  format: yaml
  label: Kredivo Checkout API
  slug: kredivo-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kredivo/refs/heads/main/openapi/kredivo-checkout-api-openapi.yml
- filename: kredivo-confirmation-api-openapi.yml
  format: yaml
  label: Kredivo Confirmation API
  slug: kredivo-confirmation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kredivo/refs/heads/main/openapi/kredivo-confirmation-api-openapi.yml
- filename: kredivo-tokenization-api-openapi.yml
  format: yaml
  label: Kredivo Tokenization API
  slug: kredivo-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kredivo/refs/heads/main/openapi/kredivo-tokenization-api-openapi.yml
- filename: kredivo-transactions-api-openapi.yml
  format: yaml
  label: Kredivo Transactions API
  slug: kredivo-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kredivo/refs/heads/main/openapi/kredivo-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: finaccel.co
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: kredivo.com
  spf: true
hosts:
- cert_expires: Sep 12 23:58:51 2026 GMT
  host: finaccel.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: doc.kredivo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: sandbox.kredivo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kredivo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kredivo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kredivo
provider_slug: kredivo
slug: kredivo-domain-security
source_filename: kredivo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: finaccel.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:58:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: doc.kredivo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: false\n- host: sandbox.kredivo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: finaccel.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: kredivo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kredivo/refs/heads/main/security/kredivo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Buy Now Pay Later
- BNPL
- Lending
- Consumer Credit
- Checkout
- Fintech
- E-Commerce
- Indonesia
- Southeast Asia
- Financial-Services
---
