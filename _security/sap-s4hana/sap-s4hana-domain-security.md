---
api_specs:
- filename: sap-s4hana-partners-api-openapi.yml
  format: yaml
  label: SAP S/4HANA Partners API
  slug: sap-s4hana-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/openapi/sap-s4hana-partners-api-openapi.yml
- filename: sap-s4hana-pricing-elements-api-openapi.yml
  format: yaml
  label: SAP S/4HANA Pricing Elements API
  slug: sap-s4hana-pricing-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/openapi/sap-s4hana-pricing-elements-api-openapi.yml
- filename: sap-s4hana-sales-order-items-api-openapi.yml
  format: yaml
  label: SAP S/4HANA Sales Order Items API
  slug: sap-s4hana-sales-order-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/openapi/sap-s4hana-sales-order-items-api-openapi.yml
- filename: sap-s4hana-sales-orders-api-openapi.yml
  format: yaml
  label: SAP S/4HANA Sales Orders API
  slug: sap-s4hana-sales-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/openapi/sap-s4hana-sales-orders-api-openapi.yml
- filename: sap-s4hana-schedule-lines-api-openapi.yml
  format: yaml
  label: SAP S/4HANA Schedule Lines API
  slug: sap-s4hana-schedule-lines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/openapi/sap-s4hana-schedule-lines-api-openapi.yml
- filename: sap-s4hana-text-api-openapi.yml
  format: yaml
  label: SAP S/4HANA Text API
  slug: sap-s4hana-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/openapi/sap-s4hana-text-api-openapi.yml
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
- cert_expires: Aug 12 23:59:59 2026 GMT
  host: sandbox.api.sap.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sap S4Hana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SAP S/4HANA, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SAP S/4HANA
provider_slug: sap-s4hana
slug: sap-s4hana-domain-security
source_filename: sap-s4hana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\n- host: sandbox.api.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/security/sap-s4hana-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Business Applications
- Cloud
- Enterprise Resource Planning
- ERP
- Finance
- Human Resources
- Inventory
- Logistics
- Manufacturing
- Plant Maintenance
- Procurement
- S/4HANA
- Sales
- SAP
---
