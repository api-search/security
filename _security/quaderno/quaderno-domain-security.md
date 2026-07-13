---
api_specs:
- filename: quaderno-openapi.yml
  format: yaml
  label: Quaderno Invoices API
  slug: quaderno-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-openapi.yml
- filename: quaderno-openapi.yml
  format: yaml
  label: Quaderno Credits API
  slug: quaderno-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-openapi.yml
- filename: quaderno-openapi.yml
  format: yaml
  label: Quaderno Estimates API
  slug: quaderno-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-openapi.yml
- filename: quaderno-openapi.yml
  format: yaml
  label: Quaderno Expenses API
  slug: quaderno-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-openapi.yml
- filename: quaderno-openapi.yml
  format: yaml
  label: Quaderno Contacts API
  slug: quaderno-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-openapi.yml
- filename: quaderno-openapi.yml
  format: yaml
  label: Quaderno Items API
  slug: quaderno-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-openapi.yml
- filename: quaderno-openapi.yml
  format: yaml
  label: Quaderno Taxes API
  slug: quaderno-taxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-openapi.yml
- filename: quaderno-openapi.yml
  format: yaml
  label: Quaderno Payments API
  slug: quaderno-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-openapi.yml
- filename: quaderno-openapi.yml
  format: yaml
  label: Quaderno Transactions API
  slug: quaderno-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-openapi.yml
- filename: quaderno-openapi.yml
  format: yaml
  label: Quaderno Checkout API
  slug: quaderno-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-openapi.yml
- filename: quaderno-openapi.yml
  format: yaml
  label: Quaderno Webhooks API
  slug: quaderno-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/openapi/quaderno-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: quaderno.io
  spf: true
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  dmarc: false
  dnssec: false
  domain: quadernoapp.com
  spf: true
hosts:
- cert_expires: Aug 21 05:59:45 2026 GMT
  host: quaderno.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 07:10:03 2026 GMT
  host: developers.quaderno.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: account_name.quadernoapp.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''account_nam'
kind: domain-security
layout: security
method: probed
name: Quaderno Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quaderno, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Quaderno
provider_slug: quaderno
slug: quaderno-domain-security
source_filename: quaderno-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quaderno.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 05:59:45 2026 GMT\n  hsts: false\n- host: developers.quaderno.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 07:10:03 2026 GMT\n  hsts: false\n- host: account_name.quadernoapp.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''account_nam'\n  hsts: null\ndomains:\n- domain: quaderno.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: quadernoapp.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"\
  amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/security/quaderno-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Tax Compliance
- Sales Tax
- VAT
- Invoicing
- Billing
- FinTech
---
