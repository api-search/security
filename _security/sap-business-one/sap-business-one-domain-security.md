---
api_specs:
- filename: sap-business-one-businesspartners-api-openapi.yml
  format: yaml
  label: SAP Business One BusinessPartners API
  slug: sap-business-one-businesspartners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-business-one/refs/heads/main/openapi/sap-business-one-businesspartners-api-openapi.yml
- filename: sap-business-one-businesspartners-cardcode-api-openapi.yml
  format: yaml
  label: SAP Business One BusinessPartners('{CardCode}') API
  slug: sap-business-one-businesspartners-cardcode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-business-one/refs/heads/main/openapi/sap-business-one-businesspartners-cardcode-api-openapi.yml
- filename: sap-business-one-companyservice-getcompanyinfo-api-openapi.yml
  format: yaml
  label: SAP Business One CompanyService GetCompanyInfo API
  slug: sap-business-one-companyservice-getcompanyinfo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-business-one/refs/heads/main/openapi/sap-business-one-companyservice-getcompanyinfo-api-openapi.yml
- filename: sap-business-one-invoices-api-openapi.yml
  format: yaml
  label: SAP Business One Invoices API
  slug: sap-business-one-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-business-one/refs/heads/main/openapi/sap-business-one-invoices-api-openapi.yml
- filename: sap-business-one-items-api-openapi.yml
  format: yaml
  label: SAP Business One Items API
  slug: sap-business-one-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-business-one/refs/heads/main/openapi/sap-business-one-items-api-openapi.yml
- filename: sap-business-one-login-api-openapi.yml
  format: yaml
  label: SAP Business One Login API
  slug: sap-business-one-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-business-one/refs/heads/main/openapi/sap-business-one-login-api-openapi.yml
- filename: sap-business-one-logout-api-openapi.yml
  format: yaml
  label: SAP Business One Logout API
  slug: sap-business-one-logout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-business-one/refs/heads/main/openapi/sap-business-one-logout-api-openapi.yml
- filename: sap-business-one-orders-api-openapi.yml
  format: yaml
  label: SAP Business One Orders API
  slug: sap-business-one-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-business-one/refs/heads/main/openapi/sap-business-one-orders-api-openapi.yml
- filename: sap-business-one-orders-docentry-api-openapi.yml
  format: yaml
  label: SAP Business One Orders({DocEntry}) API
  slug: sap-business-one-orders-docentry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-business-one/refs/heads/main/openapi/sap-business-one-orders-docentry-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sap.com
  spf: true
hosts:
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
name: Sap Business One Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SAP Business One, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SAP Business One
provider_slug: sap-business-one
slug: sap-business-one-domain-security
source_filename: sap-business-one-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: null\n- host: help.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-business-one/refs/heads/main/security/sap-business-one-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ERP
- Enterprise Resource Planning
- Accounting
- Inventory Management
- CRM
- Small Business
- Midsize Business
- SAP
---
