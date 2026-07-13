---
api_specs:
- filename: sap-business-one-service-layer-openapi.yml
  format: yaml
  label: SAP Business One Service Layer API
  slug: sap-business-one-service-layer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-business-one-service-layer-openapi.yml
- filename: sap-s4hana-cloud-business-partner-openapi.yml
  format: yaml
  label: SAP S/4HANA Cloud API
  slug: sap-s4hana-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-s4hana-cloud-business-partner-openapi.yml
- filename: sap-event-mesh-asyncapi.yml
  format: yaml
  label: SAP Event Mesh API
  slug: sap-event-mesh-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/asyncapi/sap-event-mesh-asyncapi.yml
- filename: sap-ai-core-openapi.yml
  format: yaml
  label: SAP AI Core API
  slug: sap-ai-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-ai-core-openapi.yml
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
