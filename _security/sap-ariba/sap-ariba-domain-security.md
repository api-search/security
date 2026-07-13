---
api_specs:
- filename: sap-ariba-procurement-api.yml
  format: yaml
  label: SAP Ariba Procurement API
  slug: sap-ariba-procurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/openapi/sap-ariba-procurement-api.yml
- filename: openapi.json
  format: json
  label: SAP Ariba Sourcing API
  slug: sap-ariba-sourcing-api
  spec_type: OpenAPI
  url: https://developer.ariba.com/api/sourcing/openapi.json
- filename: openapi.json
  format: json
  label: SAP Ariba Supplier Management API
  slug: sap-ariba-supplier-management-api
  spec_type: OpenAPI
  url: https://developer.ariba.com/api/supplier/openapi.json
- filename: openapi.json
  format: json
  label: SAP Ariba Contract Management API
  slug: sap-ariba-contract-management-api
  spec_type: OpenAPI
  url: https://developer.ariba.com/api/contracts/openapi.json
- filename: openapi.json
  format: json
  label: SAP Ariba Analytical Reporting API
  slug: sap-ariba-analytical-reporting-api
  spec_type: OpenAPI
  url: https://developer.ariba.com/api/analytics/openapi.json
- filename: openapi.json
  format: json
  label: SAP Ariba Invoice Management API
  slug: sap-ariba-invoice-management-api
  spec_type: OpenAPI
  url: https://developer.ariba.com/api/invoices/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sap.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ariba.com
  spf: true
hosts:
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: api.sap.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 22 23:59:59 2027 GMT
  host: developer.ariba.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 22 23:59:59 2027 GMT
  host: openapi.ariba.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sap Ariba Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SAP Ariba, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SAP Ariba
provider_slug: sap-ariba
slug: sap-ariba-domain-security
source_filename: sap-ariba-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\n- host: developer.ariba.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: openapi.ariba.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: sap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ariba.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/security/sap-ariba-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
---
