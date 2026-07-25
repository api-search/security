---
api_specs:
- filename: orbii-business-category-assignment-api-openapi.yml
  format: yaml
  label: Orbii Business Category Assignment API
  slug: orbii-business-category-assignment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-business-category-assignment-api-openapi.yml
- filename: orbii-categories-api-openapi.yml
  format: yaml
  label: Orbii Categories API
  slug: orbii-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-categories-api-openapi.yml
- filename: orbii-clients-api-openapi.yml
  format: yaml
  label: Orbii Clients API
  slug: orbii-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-clients-api-openapi.yml
- filename: orbii-company-management-api-openapi.yml
  format: yaml
  label: Orbii Company Management API
  slug: orbii-company-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-company-management-api-openapi.yml
- filename: orbii-data-check-api-openapi.yml
  format: yaml
  label: Orbii Data Check API
  slug: orbii-data-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-data-check-api-openapi.yml
- filename: orbii-general-api-openapi.yml
  format: yaml
  label: Orbii General API
  slug: orbii-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-general-api-openapi.yml
- filename: orbii-ibans-api-openapi.yml
  format: yaml
  label: Orbii IBANs API
  slug: orbii-ibans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-ibans-api-openapi.yml
- filename: orbii-invoices-api-openapi.yml
  format: yaml
  label: Orbii Invoices API
  slug: orbii-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-invoices-api-openapi.yml
- filename: orbii-kpis-api-openapi.yml
  format: yaml
  label: Orbii KPIs API
  slug: orbii-kpis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-kpis-api-openapi.yml
- filename: orbii-lending-actions-api-openapi.yml
  format: yaml
  label: Orbii Lending Actions API
  slug: orbii-lending-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-lending-actions-api-openapi.yml
- filename: orbii-merchants-api-openapi.yml
  format: yaml
  label: Orbii Merchants API
  slug: orbii-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-merchants-api-openapi.yml
- filename: orbii-pdfs-api-openapi.yml
  format: yaml
  label: Orbii PDFs API
  slug: orbii-pdfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-pdfs-api-openapi.yml
- filename: orbii-risk-assessment-api-openapi.yml
  format: yaml
  label: Orbii Risk Assessment API
  slug: orbii-risk-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-risk-assessment-api-openapi.yml
- filename: orbii-subcategories-api-openapi.yml
  format: yaml
  label: Orbii Subcategories API
  slug: orbii-subcategories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-subcategories-api-openapi.yml
- filename: orbii-transactions-api-openapi.yml
  format: yaml
  label: Orbii Transactions API
  slug: orbii-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: orbii.ai
  spf: true
hosts:
- host: orbii.ai
  https: false
- cert_expires: Oct  4 17:53:09 2026 GMT
  host: api.docs.orbii.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:37:21 2026 GMT
  host: api.orbii.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orbii Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orbii, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Orbii
provider_slug: orbii
slug: orbii-domain-security
source_filename: orbii-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orbii.ai\n  https: false\n- host: api.docs.orbii.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 17:53:09 2026 GMT\n  hsts: false\n- host: api.orbii.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:37:21 2026 GMT\n  hsts: false\ndomains:\n- domain: orbii.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/security/orbii-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Ai
- Lending
- Credit
- Fintech
- Underwriting
- Banking
- SME
- Embedded Finance
- MENA
- Risk
---
