---
api_specs:
- filename: resolve-access-keys-api-openapi.yml
  format: yaml
  label: Resolve Access Keys API
  slug: resolve-access-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-access-keys-api-openapi.yml
- filename: resolve-charges-api-openapi.yml
  format: yaml
  label: Resolve Charges API
  slug: resolve-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-charges-api-openapi.yml
- filename: resolve-credit-notes-api-openapi.yml
  format: yaml
  label: Resolve Credit Notes API
  slug: resolve-credit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-credit-notes-api-openapi.yml
- filename: resolve-customers-api-openapi.yml
  format: yaml
  label: Resolve Customers API
  slug: resolve-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-customers-api-openapi.yml
- filename: resolve-invoices-api-openapi.yml
  format: yaml
  label: Resolve Invoices API
  slug: resolve-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-invoices-api-openapi.yml
- filename: resolve-merchants-api-openapi.yml
  format: yaml
  label: Resolve Merchants API
  slug: resolve-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-merchants-api-openapi.yml
- filename: resolve-orders-api-openapi.yml
  format: yaml
  label: Resolve Orders API
  slug: resolve-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-orders-api-openapi.yml
- filename: resolve-payments-api-openapi.yml
  format: yaml
  label: Resolve Payments API
  slug: resolve-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-payments-api-openapi.yml
- filename: resolve-payout-transactions-api-openapi.yml
  format: yaml
  label: Resolve Payout Transactions API
  slug: resolve-payout-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-payout-transactions-api-openapi.yml
- filename: resolve-payouts-api-openapi.yml
  format: yaml
  label: Resolve Payouts API
  slug: resolve-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-payouts-api-openapi.yml
- filename: resolve-shipments-api-openapi.yml
  format: yaml
  label: Resolve Shipments API
  slug: resolve-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-shipments-api-openapi.yml
- filename: resolve-webhooks-api-openapi.yml
  format: yaml
  label: Resolve Webhooks API
  slug: resolve-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: resolvepay.com
  spf: true
hosts:
- cert_expires: Oct 14 05:15:23 2026 GMT
  host: resolvepay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 17:38:41 2026 GMT
  host: docs.resolvepay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 15:58:32 2026 GMT
  host: app.resolvepay.com
  hsts: true
  hsts_max_age: 5184000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Resolve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Resolve, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Resolve
provider_slug: resolve
slug: resolve-domain-security
source_filename: resolve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: resolvepay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 05:15:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.resolvepay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 17:38:41 2026 GMT\n  hsts: false\n- host: app.resolvepay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 15:58:32 2026 GMT\n  hsts: true\n  hsts_max_age: 5184000\ndomains:\n- domain: resolvepay.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/security/resolve-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Payments
- B2B
- Net Terms
- Credit
- Invoicing
- Financing
- Embedded Finance
---
