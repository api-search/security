---
api_specs:
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Customer Invoicing API
  slug: pennylane-customer-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Supplier Invoicing API
  slug: pennylane-supplier-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Accounting & Ledger API
  slug: pennylane-accounting-ledger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Accounting Exports API
  slug: pennylane-accounting-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Banking API
  slug: pennylane-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Customers & Suppliers API
  slug: pennylane-customers-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Products Catalog API
  slug: pennylane-products-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Quotes API
  slug: pennylane-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Billing Subscriptions API
  slug: pennylane-billing-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Direct Debit Mandates API
  slug: pennylane-mandates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Change Events API
  slug: pennylane-change-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane E-Invoicing (Plateforme Agréée) API
  slug: pennylane-einvoicing-pa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
description: ''
domains:
- domain: pennylane.com
  notes: French fintech (Pennylane SAS, Paris). Marketing on www.pennylane.com; app + API on app.pennylane.com; developer docs on pennylane.readme.io.
hosts:
- cert_expires: Aug 30 12:27:21 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: app.pennylane.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  note: API base host (https://app.pennylane.com/api/external/v2) and OAuth endpoints. Returns 401 without a valid Bearer token.
  server: cloudflare
  tls_version: TLSv1.3
- cert_expires: Aug 30 00:44:03 2026 GMT
  cert_issuer: Let's Encrypt (YE2)
  host: www.pennylane.com
  https: true
  note: Primary marketing site.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pennylane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pennylane, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Pennylane
provider_slug: pennylane
slug: pennylane-domain-security
source_filename: pennylane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.pennylane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (WE1)\n  cert_expires: Aug 30 12:27:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  server: cloudflare\n  note: API base host (https://app.pennylane.com/api/external/v2) and OAuth endpoints. Returns 401 without a valid Bearer token.\n- host: www.pennylane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Let's Encrypt (YE2)\n  cert_expires: Aug 30 00:44:03 2026 GMT\n  note: Primary marketing site.\ndomains:\n- domain: pennylane.com\n  notes: French fintech (Pennylane SAS, Paris). Marketing on www.pennylane.com; app + API on app.pennylane.com; developer docs on pennylane.readme.io.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/security/pennylane-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Accounting
- Invoicing
- Fintech
- Financial Data
- Banking
- France
- SME
---
