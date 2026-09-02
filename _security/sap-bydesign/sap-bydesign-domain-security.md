---
api_specs:
- filename: sap-bydesign-analytics-api-openapi.yml
  format: yaml
  label: SAP Business ByDesign Analytics API
  slug: sap-bydesign-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bydesign/refs/heads/main/openapi/sap-bydesign-analytics-api-openapi.yml
- filename: sap-bydesign-crm-api-openapi.yml
  format: yaml
  label: SAP Business ByDesign CRM API
  slug: sap-bydesign-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bydesign/refs/heads/main/openapi/sap-bydesign-crm-api-openapi.yml
- filename: sap-bydesign-financials-api-openapi.yml
  format: yaml
  label: SAP Business ByDesign Financials API
  slug: sap-bydesign-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bydesign/refs/heads/main/openapi/sap-bydesign-financials-api-openapi.yml
- filename: sap-bydesign-master-data-api-openapi.yml
  format: yaml
  label: SAP Business ByDesign Master Data API
  slug: sap-bydesign-master-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bydesign/refs/heads/main/openapi/sap-bydesign-master-data-api-openapi.yml
- filename: sap-bydesign-procurement-api-openapi.yml
  format: yaml
  label: SAP Business ByDesign Procurement API
  slug: sap-bydesign-procurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bydesign/refs/heads/main/openapi/sap-bydesign-procurement-api-openapi.yml
- filename: sap-bydesign-projects-api-openapi.yml
  format: yaml
  label: SAP Business ByDesign Projects API
  slug: sap-bydesign-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bydesign/refs/heads/main/openapi/sap-bydesign-projects-api-openapi.yml
- filename: sap-bydesign-sales-api-openapi.yml
  format: yaml
  label: SAP Business ByDesign Sales API
  slug: sap-bydesign-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bydesign/refs/heads/main/openapi/sap-bydesign-sales-api-openapi.yml
- filename: sap-bydesign-supply-chain-api-openapi.yml
  format: yaml
  label: SAP Business ByDesign Supply Chain API
  slug: sap-bydesign-supply-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bydesign/refs/heads/main/openapi/sap-bydesign-supply-chain-api-openapi.yml
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
- cert_expires: Sep 22 23:53:07 2026 GMT
  host: community.sap.com
  hsts: false
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
name: Sap Bydesign Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SAP Business ByDesign, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SAP Business ByDesign
provider_slug: sap-bydesign
slug: sap-bydesign-domain-security
source_filename: sap-bydesign-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: null\n- host: community.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:53:07 2026 GMT\n  hsts: false\n- host: help.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-bydesign/refs/heads/main/security/sap-bydesign-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ERP
- Cloud
- Mid-Market
- Financials
- CRM
- Procurement
- Supply Chain
- Project Management
- OData
- SOAP
- SAP
---
