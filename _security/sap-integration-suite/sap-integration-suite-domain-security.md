---
api_specs:
- filename: sap-integration-suite-cloud-integration-openapi.yml
  format: yaml
  label: SAP Cloud Integration API
  slug: sap-cloud-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-integration-suite/refs/heads/main/openapi/sap-integration-suite-cloud-integration-openapi.yml
- filename: sap-integration-suite-api-management-openapi.yml
  format: yaml
  label: SAP API Management API
  slug: sap-api-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-integration-suite/refs/heads/main/openapi/sap-integration-suite-api-management-openapi.yml
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
name: Sap Integration Suite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SAP Integration Suite, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SAP Integration Suite
provider_slug: sap-integration-suite
slug: sap-integration-suite-domain-security
source_filename: sap-integration-suite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\n- host: www.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: null\n- host: help.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-integration-suite/refs/heads/main/security/sap-integration-suite-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Management
- Cloud Integration
- Enterprise Integration
- Event Mesh
- iPaaS
- SAP
- SAP BTP
---
