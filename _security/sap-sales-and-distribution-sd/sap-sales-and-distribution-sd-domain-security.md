---
api_specs:
- filename: sap-sd-sales-order-openapi.yml
  format: yaml
  label: Sales Order API
  slug: sales-order
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-sales-order-openapi.yml
- filename: sap-sd-customer-master-data-openapi.yml
  format: yaml
  label: Customer Master Data API
  slug: customer-master-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-customer-master-data-openapi.yml
- filename: sap-sd-outbound-delivery-openapi.yml
  format: yaml
  label: Outbound Delivery API
  slug: outbound-delivery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-outbound-delivery-openapi.yml
- filename: sap-sd-billing-document-openapi.yml
  format: yaml
  label: Billing Document API
  slug: billing-document
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-billing-document-openapi.yml
- filename: sap-sd-pricing-openapi.yml
  format: yaml
  label: Pricing API
  slug: pricing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-pricing-openapi.yml
- filename: sap-sd-sales-quotation-openapi.yml
  format: yaml
  label: Sales Quotation API
  slug: sales-quotation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-sales-quotation-openapi.yml
- filename: sap-sd-credit-management-openapi.yml
  format: yaml
  label: Credit Management API
  slug: credit-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-credit-management-openapi.yml
- filename: sap-sd-material-master-openapi.yml
  format: yaml
  label: Material Master API
  slug: material-master
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-material-master-openapi.yml
- filename: sap-sd-credit-memo-request-openapi.yml
  format: yaml
  label: Credit Memo Request API
  slug: credit-memo-request
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-credit-memo-request-openapi.yml
- filename: sap-sd-debit-memo-request-openapi.yml
  format: yaml
  label: Debit Memo Request API
  slug: debit-memo-request
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-debit-memo-request-openapi.yml
- filename: sap-sd-sales-contract-openapi.yml
  format: yaml
  label: Sales Contract API
  slug: sales-contract
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-sales-contract-openapi.yml
- filename: sap-sd-sales-inquiry-openapi.yml
  format: yaml
  label: Sales Inquiry API
  slug: sales-inquiry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-sales-inquiry-openapi.yml
- filename: sap-sd-sales-scheduling-agreement-openapi.yml
  format: yaml
  label: Sales Scheduling Agreement API
  slug: sales-scheduling-agreement
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-sales-scheduling-agreement-openapi.yml
- filename: sap-sd-customer-return-openapi.yml
  format: yaml
  label: Customer Return API
  slug: customer-return
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-customer-return-openapi.yml
- filename: sap-sd-customer-returns-delivery-openapi.yml
  format: yaml
  label: Customer Returns Delivery API
  slug: customer-returns-delivery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-customer-returns-delivery-openapi.yml
- filename: sap-sd-customer-material-openapi.yml
  format: yaml
  label: Customer Material API
  slug: customer-material
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-customer-material-openapi.yml
- filename: sap-sd-inbound-delivery-openapi.yml
  format: yaml
  label: Inbound Delivery API
  slug: inbound-delivery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-inbound-delivery-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sap.com
  spf: true
hosts:
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: api.sap.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: www.sap.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 23:59:59 2026 GMT
  host: sandbox.api.sap.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sap Sales And Distribution Sd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SAP Sales and Distribution (SD), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SAP Sales and Distribution (SD)
provider_slug: sap-sales-and-distribution-sd
slug: sap-sales-and-distribution-sd-domain-security
source_filename: sap-sales-and-distribution-sd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\n- host: www.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: null\n- host: sandbox.api.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/security/sap-sales-and-distribution-sd-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Distribution
- ERP
- OData
- S/4HANA
- Sales
- SAP
---
