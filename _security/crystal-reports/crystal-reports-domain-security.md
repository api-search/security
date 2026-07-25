---
api_specs:
- filename: crystal-reports-authentication-api-openapi.yml
  format: yaml
  label: Crystal Reports Authentication API
  slug: crystal-reports-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/openapi/crystal-reports-authentication-api-openapi.yml
- filename: crystal-reports-export-api-openapi.yml
  format: yaml
  label: Crystal Reports Export API
  slug: crystal-reports-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/openapi/crystal-reports-export-api-openapi.yml
- filename: crystal-reports-instances-api-openapi.yml
  format: yaml
  label: Crystal Reports Instances API
  slug: crystal-reports-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/openapi/crystal-reports-instances-api-openapi.yml
- filename: crystal-reports-metadata-api-openapi.yml
  format: yaml
  label: Crystal Reports Metadata API
  slug: crystal-reports-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/openapi/crystal-reports-metadata-api-openapi.yml
- filename: crystal-reports-odata-api-openapi.yml
  format: yaml
  label: Crystal Reports OData API
  slug: crystal-reports-odata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/openapi/crystal-reports-odata-api-openapi.yml
- filename: crystal-reports-reports-api-openapi.yml
  format: yaml
  label: Crystal Reports Reports API
  slug: crystal-reports-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/openapi/crystal-reports-reports-api-openapi.yml
- filename: crystal-reports-repository-api-openapi.yml
  format: yaml
  label: Crystal Reports Repository API
  slug: crystal-reports-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/openapi/crystal-reports-repository-api-openapi.yml
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
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: www.sap.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crystal Reports Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crystal Reports, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Crystal Reports
provider_slug: crystal-reports
slug: crystal-reports-domain-security
source_filename: crystal-reports-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\n- host: help.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: sap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/security/crystal-reports-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
---
