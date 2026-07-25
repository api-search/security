---
api_specs:
- filename: earnipay-app-api-openapi.yml
  format: yaml
  label: Earnipay App API
  slug: earnipay-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/earnipay/refs/heads/main/openapi/earnipay-app-api-openapi.yml
- filename: earnipay-app-provider-api-openapi.yml
  format: yaml
  label: Earnipay APP Provider API
  slug: earnipay-app-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/earnipay/refs/heads/main/openapi/earnipay-app-provider-api-openapi.yml
- filename: earnipay-authentication-api-openapi.yml
  format: yaml
  label: Earnipay Authentication API
  slug: earnipay-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/earnipay/refs/heads/main/openapi/earnipay-authentication-api-openapi.yml
- filename: earnipay-bank-api-openapi.yml
  format: yaml
  label: Earnipay Bank API
  slug: earnipay-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/earnipay/refs/heads/main/openapi/earnipay-bank-api-openapi.yml
- filename: earnipay-business-api-openapi.yml
  format: yaml
  label: Earnipay Business API
  slug: earnipay-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/earnipay/refs/heads/main/openapi/earnipay-business-api-openapi.yml
- filename: earnipay-customers-api-openapi.yml
  format: yaml
  label: Earnipay Customers API
  slug: earnipay-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/earnipay/refs/heads/main/openapi/earnipay-customers-api-openapi.yml
- filename: earnipay-invoices-api-openapi.yml
  format: yaml
  label: Earnipay Invoices API
  slug: earnipay-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/earnipay/refs/heads/main/openapi/earnipay-invoices-api-openapi.yml
- filename: earnipay-irn-generator-api-openapi.yml
  format: yaml
  label: Earnipay IRN Generator API
  slug: earnipay-irn-generator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/earnipay/refs/heads/main/openapi/earnipay-irn-generator-api-openapi.yml
- filename: earnipay-payment-details-api-openapi.yml
  format: yaml
  label: Earnipay Payment Details API
  slug: earnipay-payment-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/earnipay/refs/heads/main/openapi/earnipay-payment-details-api-openapi.yml
- filename: earnipay-products-api-openapi.yml
  format: yaml
  label: Earnipay Products API
  slug: earnipay-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/earnipay/refs/heads/main/openapi/earnipay-products-api-openapi.yml
- filename: earnipay-qr-code-generator-api-openapi.yml
  format: yaml
  label: Earnipay QR Code Generator API
  slug: earnipay-qr-code-generator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/earnipay/refs/heads/main/openapi/earnipay-qr-code-generator-api-openapi.yml
- filename: earnipay-team-api-openapi.yml
  format: yaml
  label: Earnipay Team API
  slug: earnipay-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/earnipay/refs/heads/main/openapi/earnipay-team-api-openapi.yml
- filename: earnipay-users-api-openapi.yml
  format: yaml
  label: Earnipay Users API
  slug: earnipay-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/earnipay/refs/heads/main/openapi/earnipay-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: earnipay.com
  spf: true
hosts:
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: earnipay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 21:40:17 2026 GMT
  host: docs.earnipay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 20:15:15 2026 GMT
  host: e-invoicing.earnipay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Earnipay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Earnipay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Earnipay
provider_slug: earnipay
slug: earnipay-domain-security
source_filename: earnipay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: earnipay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: false\n- host: docs.earnipay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 21:40:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: e-invoicing.earnipay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 20:15:15 2026 GMT\n  hsts: null\ndomains:\n- domain: earnipay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/earnipay/refs/heads/main/security/earnipay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-Invoicing
- Invoicing
- FIRS
- NRS
- Tax
- Compliance
- Fintech
- Nigeria
- Payments
- Financial Services
---
