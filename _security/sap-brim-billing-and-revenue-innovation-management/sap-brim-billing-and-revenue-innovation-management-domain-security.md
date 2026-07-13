---
api_specs:
- filename: overview
  format: yaml
  label: SAP Convergent Charging API
  slug: sap-convergent-charging-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/convergent_charging/overview
- filename: overview
  format: yaml
  label: SAP Convergent Invoicing API
  slug: sap-convergent-invoicing-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/convergent_invoicing/overview
- filename: overview
  format: yaml
  label: SAP Subscription Billing API
  slug: sap-subscription-billing-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/subscription_billing/overview
- filename: overview
  format: yaml
  label: SAP Contract Accounts Receivable and Payable API
  slug: sap-contract-accounts-receivable-and-payable-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/fica/overview
- filename: overview
  format: yaml
  label: SAP BRIM Usage Data Intake API
  slug: sap-brim-usage-data-intake-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/usage_data_intake/overview
- filename: overview
  format: yaml
  label: SAP Revenue Accounting and Reporting API
  slug: sap-revenue-accounting-and-reporting-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/revenue_accounting/overview
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
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: help.sap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sap Brim Billing And Revenue Innovation Management Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SAP BRIM (Billing and Revenue Innovation Management), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SAP BRIM (Billing and Revenue Innovation Management)
provider_slug: sap-brim-billing-and-revenue-innovation-management
slug: sap-brim-billing-and-revenue-innovation-management-domain-security
source_filename: sap-brim-billing-and-revenue-innovation-management-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\n- host: www.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: null\n- host: help.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-brim-billing-and-revenue-innovation-management/refs/heads/main/security/sap-brim-billing-and-revenue-innovation-management-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Billing
- Enterprise
- Order to Cash
- Revenue Management
- SAP
- Subscription Management
- Usage-Based Pricing
---
