---
api_specs:
- filename: hapi-fhir-fhir-api-openapi.yml
  format: yaml
  label: HAPI FHIR Fhir API
  slug: hapi-fhir-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hapi-fhir/refs/heads/main/openapi/hapi-fhir-fhir-api-openapi.yml
- filename: hapi-fhir-patient-api-openapi.yml
  format: yaml
  label: HAPI FHIR Patient API
  slug: hapi-fhir-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hapi-fhir/refs/heads/main/openapi/hapi-fhir-patient-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hapifhir.io
  spf: false
hosts:
- cert_expires: Dec  3 05:31:12 2026 GMT
  host: hapifhir.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hapi Fhir Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HAPI FHIR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: HAPI FHIR
provider_slug: hapi-fhir
slug: hapi-fhir-domain-security
source_filename: hapi-fhir-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hapifhir.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  3 05:31:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hapifhir.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hapi-fhir/refs/heads/main/security/hapi-fhir-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Healthcare
- Interoperability
- Open Source
- Java
- FHIR
---
