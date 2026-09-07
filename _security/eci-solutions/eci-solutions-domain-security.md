---
api_specs:
- filename: eci-solutions-erp-v2-1-openapi.json
  format: json
  label: ECI Manufacturing ERP API
  slug: eci-solutions-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-erp-v2-1-openapi.json
- filename: eci-solutions-jobboss2-openapi.json
  format: json
  label: JobBOSS² Public API
  slug: eci-solutions-jobboss2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-jobboss2-openapi.json
- filename: eci-solutions-m1-openapi.json
  format: json
  label: M1 Public API
  slug: eci-solutions-m1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-m1-openapi.json
- filename: eci-solutions-management-openapi.json
  format: json
  label: ECI MFG Integration Management API
  slug: eci-solutions-integration-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-management-openapi.json
- filename: eci-solutions-authentication-openapi.json
  format: json
  label: ECI Authentication API
  slug: eci-solutions-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-authentication-openapi.json
- filename: eci-solutions-payment-openapi.json
  format: json
  label: ECI MFG Payment API
  slug: eci-solutions-payment
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-payment-openapi.json
- filename: eci-solutions-financial-v2-openapi.json
  format: json
  label: ECI Financial Integration API
  slug: eci-solutions-financial
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-financial-v2-openapi.json
- filename: eci-solutions-ecommerce-openapi.json
  format: json
  label: ECI EvolutionX Ecommerce API
  slug: eci-solutions-ecommerce
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-ecommerce-openapi.json
- filename: eci-solutions-einvoice-openapi.json
  format: json
  label: ECI Einvoice API
  slug: eci-solutions-einvoice
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-einvoice-openapi.json
- filename: eci-solutions-shipping-openapi.json
  format: json
  label: ECI Shipping API
  slug: eci-solutions-shipping
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-shipping-openapi.json
- filename: eci-solutions-currency-openapi.json
  format: json
  label: ECI Currency Data API
  slug: eci-solutions-currency
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-currency-openapi.json
- filename: eci-solutions-apar-commerce-openapi.json
  format: json
  label: ECI AP/AR Commerce Automation API
  slug: eci-solutions-apar-commerce
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-apar-commerce-openapi.json
- filename: eci-solutions-office-openapi.json
  format: json
  label: ECI Office Integration API
  slug: eci-solutions-office
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-office-openapi.json
- filename: eci-solutions-notification-openapi.json
  format: json
  label: ECI Notification API
  slug: eci-solutions-notification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-notification-openapi.json
- filename: eci-solutions-lasso-crm-openapi.yml
  format: yaml
  label: Lasso CRM API
  slug: eci-solutions-lasso-crm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-lasso-crm-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ecisolutions.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: ecimanufacturing.com
  spf: false
hosts:
- cert_expires: Oct 21 22:42:37 2026 GMT
  host: www.ecisolutions.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: integrations.ecimanufacturing.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: api-erp.integrations.ecimanufacturing.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Eci Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ECI Solutions, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ECI Solutions
provider_slug: eci-solutions
slug: eci-solutions-domain-security
source_filename: eci-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ecisolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 22:42:37 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: integrations.ecimanufacturing.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: false\n- host: api-erp.integrations.ecimanufacturing.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ecisolutions.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ecimanufacturing.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/security/eci-solutions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- Building Supply
- Business Management
- CRM
- Construction
- Distribution
- E-Commerce
- ERP
- Field Service
- Inventory
- Manufacturing
- Payments
- Retail
- Shipping
---
