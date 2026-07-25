---
api_specs:
- filename: infoway-fhir-terminology-service-api-openapi.json
  format: json
  label: Infoway FHIR Terminology Service API
  slug: infoway-fhir-terminology-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/infoway-fhir-terminology-service-api-openapi.json
- filename: infoway-terminology-service-api-openapi.json
  format: json
  label: Infoway Terminology Service API
  slug: infoway-terminology-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/infoway-terminology-service-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: infoway-inforoute.ca
  spf: false
hosts:
- cert_expires: Aug 29 19:48:47 2026 GMT
  host: www.infoway-inforoute.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 31 07:45:56 2026 GMT
  host: termapi.infoway-inforoute.ca
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Canada Health Infoway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canada Health Infoway, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Canada Health Infoway
provider_slug: canada-health-infoway
slug: canada-health-infoway-domain-security
source_filename: canada-health-infoway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.infoway-inforoute.ca\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 29 19:48:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: termapi.infoway-inforoute.ca\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 31 07:45:56 2026 GMT\n  hsts: null\ndomains:\n- domain: infoway-inforoute.ca\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/security/canada-health-infoway-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Healthcare
- Canada
- FHIR
- HL7
- Interoperability
- Terminology
- National Health System
- Digital Health
- Standards
- CA Core
---
