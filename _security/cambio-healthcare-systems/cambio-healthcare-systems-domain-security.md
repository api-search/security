---
api_specs:
- filename: cambio-healthcare-systems-booked-appointments-api-openapi.yml
  format: yaml
  label: Cambio Healthcare Systems Booked Appointments API
  slug: cambio-healthcare-systems-booked-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cambio-healthcare-systems/refs/heads/main/openapi/cambio-healthcare-systems-booked-appointments-api-openapi.yml
- filename: cambio-healthcare-systems-default-api-openapi.yml
  format: yaml
  label: Cambio Healthcare Systems * API
  slug: cambio-healthcare-systems-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cambio-healthcare-systems/refs/heads/main/openapi/cambio-healthcare-systems-default-api-openapi.yml
- filename: cambio-healthcare-systems-payment-notice-api-openapi.yml
  format: yaml
  label: Cambio Healthcare Systems Payment Notice API
  slug: cambio-healthcare-systems-payment-notice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cambio-healthcare-systems/refs/heads/main/openapi/cambio-healthcare-systems-payment-notice-api-openapi.yml
- filename: cambio-healthcare-systems-protocol-api-openapi.yml
  format: yaml
  label: Cambio Healthcare Systems Protocol API
  slug: cambio-healthcare-systems-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cambio-healthcare-systems/refs/heads/main/openapi/cambio-healthcare-systems-protocol-api-openapi.yml
- filename: cambio-healthcare-systems-well-known-api-openapi.yml
  format: yaml
  label: Cambio Healthcare Systems .well Known API
  slug: cambio-healthcare-systems-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cambio-healthcare-systems/refs/heads/main/openapi/cambio-healthcare-systems-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cambiogroup.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cambio.se
  spf: true
hosts:
- cert_expires: Nov 19 01:42:04 2026 GMT
  host: www.cambiogroup.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: developer.openservices.cambio.se
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: api.openservices.cambio.se
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Cambio Healthcare Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cambio Healthcare Systems, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Cambio Healthcare Systems
provider_slug: cambio-healthcare-systems
slug: cambio-healthcare-systems-domain-security
source_filename: cambio-healthcare-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cambiogroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 01:42:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.openservices.cambio.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.openservices.cambio.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cambiogroup.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: cambio.se\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cambio-healthcare-systems/refs/heads/main/security/cambio-healthcare-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Electronic Health Records
- EHR
- Clinical Decision Support
- FHIR
- HL7
- Interoperability
- Health IT
- Sweden
- Nordic
- Patient Data
- Medical Records
- openEHR
- SMART on FHIR
- Company
---
