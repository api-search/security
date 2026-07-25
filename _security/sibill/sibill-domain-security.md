---
api_specs:
- filename: sibill-account-api-openapi.yml
  format: yaml
  label: Sibill Account API
  slug: sibill-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-account-api-openapi.yml
- filename: sibill-category-api-openapi.yml
  format: yaml
  label: Sibill Category API
  slug: sibill-category-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-category-api-openapi.yml
- filename: sibill-company-api-openapi.yml
  format: yaml
  label: Sibill Company API
  slug: sibill-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-company-api-openapi.yml
- filename: sibill-counterpart-api-openapi.yml
  format: yaml
  label: Sibill Counterpart API
  slug: sibill-counterpart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-counterpart-api-openapi.yml
- filename: sibill-document-api-openapi.yml
  format: yaml
  label: Sibill Document API
  slug: sibill-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-document-api-openapi.yml
- filename: sibill-documentsectional-api-openapi.yml
  format: yaml
  label: Sibill DocumentSectional API
  slug: sibill-documentsectional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-documentsectional-api-openapi.yml
- filename: sibill-flow-api-openapi.yml
  format: yaml
  label: Sibill Flow API
  slug: sibill-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-flow-api-openapi.yml
- filename: sibill-payment-api-openapi.yml
  format: yaml
  label: Sibill Payment API
  slug: sibill-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-payment-api-openapi.yml
- filename: sibill-product-api-openapi.yml
  format: yaml
  label: Sibill Product API
  slug: sibill-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-product-api-openapi.yml
- filename: sibill-reconciliation-api-openapi.yml
  format: yaml
  label: Sibill Reconciliation API
  slug: sibill-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-reconciliation-api-openapi.yml
- filename: sibill-subcategory-api-openapi.yml
  format: yaml
  label: Sibill Subcategory API
  slug: sibill-subcategory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-subcategory-api-openapi.yml
- filename: sibill-transaction-api-openapi.yml
  format: yaml
  label: Sibill Transaction API
  slug: sibill-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-transaction-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sibill.com
  spf: true
hosts:
- cert_expires: Aug 24 19:10:56 2026 GMT
  host: sibill.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 10:46:03 2026 GMT
  host: docs.sibill.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 10:46:03 2026 GMT
  host: integration.sibill.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sibill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sibill, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sibill
provider_slug: sibill
slug: sibill-domain-security
source_filename: sibill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sibill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 19:10:56 2026 GMT\n  hsts: false\n- host: docs.sibill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 10:46:03 2026 GMT\n  hsts: false\n- host: integration.sibill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 10:46:03 2026 GMT\n  hsts: null\ndomains:\n- domain: sibill.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/security/sibill-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Invoicing
- Payments
- Reconciliation
- Accounting
- Banking
- SME
- Open Banking
- Electronic Invoicing
- Italy
---
