---
api_specs:
- filename: overview
  format: yaml
  label: SAP Analytics Cloud API
  slug: sap-analytics-cloud-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/API_ANALYTICS_CLOUD/overview
- filename: overview
  format: yaml
  label: SAP BusinessObjects BI Platform REST API
  slug: sap-businessobjects-bi-platform-rest-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/BOBJ_BIPLATFORM/overview
- filename: sap-bi-bw4hana-odata-openapi.yml
  format: yaml
  label: SAP BW/4HANA OData API
  slug: sap-bw4hana-odata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bi/refs/heads/main/openapi/sap-bi-bw4hana-odata-openapi.yml
- filename: overview
  format: yaml
  label: SAP Datasphere API
  slug: sap-datasphere-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/datasphere/overview
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
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: help.sap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sap Bi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SAP Business Intelligence, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SAP Business Intelligence
provider_slug: sap-bi
slug: sap-bi-domain-security
source_filename: sap-bi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\n- host: help.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-bi/refs/heads/main/security/sap-bi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Business Intelligence
- Data Visualization
- Reporting
- SAP
---
