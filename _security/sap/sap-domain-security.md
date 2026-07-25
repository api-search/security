---
api_specs:
- filename: sap-event-mesh-asyncapi.yml
  format: yaml
  label: SAP Event Mesh API
  slug: sap-event-mesh-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/asyncapi/sap-event-mesh-asyncapi.yml
- filename: sap-addresses-api-openapi.yml
  format: yaml
  label: SAP Addresses API
  slug: sap-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-addresses-api-openapi.yml
- filename: sap-artifacts-api-openapi.yml
  format: yaml
  label: SAP Artifacts API
  slug: sap-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-artifacts-api-openapi.yml
- filename: sap-authentication-api-openapi.yml
  format: yaml
  label: SAP Authentication API
  slug: sap-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-authentication-api-openapi.yml
- filename: sap-bank-accounts-api-openapi.yml
  format: yaml
  label: SAP Bank Accounts API
  slug: sap-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-bank-accounts-api-openapi.yml
- filename: sap-business-partners-api-openapi.yml
  format: yaml
  label: SAP Business Partners API
  slug: sap-business-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-business-partners-api-openapi.yml
- filename: sap-configurations-api-openapi.yml
  format: yaml
  label: SAP Configurations API
  slug: sap-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-configurations-api-openapi.yml
- filename: sap-deployments-api-openapi.yml
  format: yaml
  label: SAP Deployments API
  slug: sap-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-deployments-api-openapi.yml
- filename: sap-executions-api-openapi.yml
  format: yaml
  label: SAP Executions API
  slug: sap-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-executions-api-openapi.yml
- filename: sap-invoices-api-openapi.yml
  format: yaml
  label: SAP Invoices API
  slug: sap-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-invoices-api-openapi.yml
- filename: sap-items-api-openapi.yml
  format: yaml
  label: SAP Items API
  slug: sap-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-items-api-openapi.yml
- filename: sap-journal-entries-api-openapi.yml
  format: yaml
  label: SAP Journal Entries API
  slug: sap-journal-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-journal-entries-api-openapi.yml
- filename: sap-orders-api-openapi.yml
  format: yaml
  label: SAP Orders API
  slug: sap-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-orders-api-openapi.yml
- filename: sap-roles-api-openapi.yml
  format: yaml
  label: SAP Roles API
  slug: sap-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-roles-api-openapi.yml
- filename: sap-scenarios-api-openapi.yml
  format: yaml
  label: SAP Scenarios API
  slug: sap-scenarios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-scenarios-api-openapi.yml
- filename: sap-tax-numbers-api-openapi.yml
  format: yaml
  label: SAP Tax Numbers API
  slug: sap-tax-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-tax-numbers-api-openapi.yml
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
kind: domain-security
layout: security
method: probed
name: Sap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SAP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SAP
provider_slug: sap
slug: sap-domain-security
source_filename: sap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: sap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/security/sap-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
---
