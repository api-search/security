---
api_specs:
- filename: billecta-accounting-api-openapi.yml
  format: yaml
  label: Billecta Accounting API
  slug: billecta-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billecta/refs/heads/main/openapi/billecta-accounting-api-openapi.yml
- filename: billecta-accountingdimensions-api-openapi.yml
  format: yaml
  label: Billecta Accountingdimensions API
  slug: billecta-accountingdimensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billecta/refs/heads/main/openapi/billecta-accountingdimensions-api-openapi.yml
- filename: billecta-action-api-openapi.yml
  format: yaml
  label: Billecta Action API
  slug: billecta-action-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billecta/refs/heads/main/openapi/billecta-action-api-openapi.yml
- filename: billecta-authentication-api-openapi.yml
  format: yaml
  label: Billecta Authentication API
  slug: billecta-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billecta/refs/heads/main/openapi/billecta-authentication-api-openapi.yml
- filename: billecta-bankaccount-api-openapi.yml
  format: yaml
  label: Billecta Bankaccount API
  slug: billecta-bankaccount-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billecta/refs/heads/main/openapi/billecta-bankaccount-api-openapi.yml
- filename: billecta-bankid-api-openapi.yml
  format: yaml
  label: Billecta Bankid API
  slug: billecta-bankid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billecta/refs/heads/main/openapi/billecta-bankid-api-openapi.yml
- filename: billecta-common-api-openapi.yml
  format: yaml
  label: Billecta Common API
  slug: billecta-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billecta/refs/heads/main/openapi/billecta-common-api-openapi.yml
- filename: billecta-contractinvoice-api-openapi.yml
  format: yaml
  label: Billecta Contractinvoice API
  slug: billecta-contractinvoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billecta/refs/heads/main/openapi/billecta-contractinvoice-api-openapi.yml
- filename: billecta-creditors-api-openapi.yml
  format: yaml
  label: Billecta Creditors API
  slug: billecta-creditors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billecta/refs/heads/main/openapi/billecta-creditors-api-openapi.yml
- filename: billecta-debtors-api-openapi.yml
  format: yaml
  label: Billecta Debtors API
  slug: billecta-debtors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billecta/refs/heads/main/openapi/billecta-debtors-api-openapi.yml
- filename: billecta-invoice-api-openapi.yml
  format: yaml
  label: Billecta Invoice API
  slug: billecta-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billecta/refs/heads/main/openapi/billecta-invoice-api-openapi.yml
- filename: billecta-products-api-openapi.yml
  format: yaml
  label: Billecta Products API
  slug: billecta-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billecta/refs/heads/main/openapi/billecta-products-api-openapi.yml
- filename: billecta-search-api-openapi.yml
  format: yaml
  label: Billecta Search API
  slug: billecta-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billecta/refs/heads/main/openapi/billecta-search-api-openapi.yml
- filename: billecta-add-ons-api-openapi.yml
  format: yaml
  label: Billecta Add Ons API
  slug: billecta-add-ons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billecta/refs/heads/main/openapi/billecta-add-ons-api-openapi.yml
- filename: billecta-cost-centers-api-openapi.yml
  format: yaml
  label: Billecta Cost Centers API
  slug: billecta-cost-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billecta/refs/heads/main/openapi/billecta-cost-centers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: billecta.com
  spf: true
hosts:
- cert_expires: Nov 23 13:39:51 2026 GMT
  host: billecta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Billecta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Billecta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Billecta
provider_slug: billecta
slug: billecta-domain-security
source_filename: billecta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: billecta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 13:39:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: billecta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/billecta/refs/heads/main/security/billecta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Invoicing
- Payments
- Software-as-a-Service
- Sweden
- BusinessAutomation
---
