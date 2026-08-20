---
api_specs:
- filename: sap-fieldglass-approval-api-openapi.yml
  format: yaml
  label: SAP Fieldglass Approval API
  slug: sap-fieldglass-approval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-approval-api-openapi.yml
- filename: sap-fieldglass-audit-trail-api-openapi.yml
  format: yaml
  label: SAP Fieldglass Audit Trail API
  slug: sap-fieldglass-audit-trail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-audit-trail-api-openapi.yml
- filename: sap-fieldglass-get-data-api-openapi.yml
  format: yaml
  label: SAP Fieldglass Get Data API
  slug: sap-fieldglass-get-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-get-data-api-openapi.yml
- filename: sap-fieldglass-get-entities-api-openapi.yml
  format: yaml
  label: SAP Fieldglass Get Entities API
  slug: sap-fieldglass-get-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-get-entities-api-openapi.yml
- filename: sap-fieldglass-get-metadata-api-openapi.yml
  format: yaml
  label: SAP Fieldglass Get Metadata API
  slug: sap-fieldglass-get-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-get-metadata-api-openapi.yml
- filename: sap-fieldglass-get-providers-api-openapi.yml
  format: yaml
  label: SAP Fieldglass Get Providers API
  slug: sap-fieldglass-get-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-get-providers-api-openapi.yml
- filename: sap-fieldglass-order-confirmation-api-openapi.yml
  format: yaml
  label: SAP Fieldglass Order Confirmation API
  slug: sap-fieldglass-order-confirmation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-order-confirmation-api-openapi.yml
- filename: sap-fieldglass-reports-api-openapi.yml
  format: yaml
  label: SAP Fieldglass Reports API
  slug: sap-fieldglass-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-reports-api-openapi.yml
- filename: sap-fieldglass-results-api-openapi.yml
  format: yaml
  label: SAP Fieldglass Results API
  slug: sap-fieldglass-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-results-api-openapi.yml
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
  dmarc_policy: reject
  dnssec: false
  domain: fieldglass.net
  spf: false
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
- cert_expires: Sep 11 03:25:10 2026 GMT
  host: www.fieldglass.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sap Fieldglass Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SAP Fieldglass, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SAP Fieldglass
provider_slug: sap-fieldglass
slug: sap-fieldglass-domain-security
source_filename: sap-fieldglass-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: null\n- host: help.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.fieldglass.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 03:25:10 2026 GMT\n  hsts: false\ndomains:\n- domain: sap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fieldglass.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/security/sap-fieldglass-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Contingent Workforce
- External Talent
- HCM
- Services Procurement
- Statements of Work
- Vendor Management
- Workforce Management
---
