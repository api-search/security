---
api_specs:
- filename: orion-fhir-openapi.yml
  format: yaml
  label: Orion Health FHIR API
  slug: orion-health-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orion/refs/heads/main/openapi/orion-fhir-openapi.yml
- filename: orion-population-health-openapi.yml
  format: yaml
  label: Orion Health Population Health API
  slug: orion-health-population-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orion/refs/heads/main/openapi/orion-population-health-openapi.yml
- filename: orion-hie-openapi.yml
  format: yaml
  label: Orion Health HIE API
  slug: orion-health-hie-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orion/refs/heads/main/openapi/orion-hie-openapi.yml
- filename: orion-rhapsody-openapi.yml
  format: yaml
  label: Orion Health Rhapsody Integration API
  slug: orion-health-rhapsody-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orion/refs/heads/main/openapi/orion-rhapsody-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: orionhealth.io
  spf: false
- caa:
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: orionhealth.com
  spf: true
hosts:
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: developer.orionhealth.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 17:50:55 2026 GMT
  host: www.orionhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.orionhealth.com
  https: false
kind: domain-security
layout: security
method: probed
name: Orion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orion Health, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Orion Health
provider_slug: orion
slug: orion-domain-security
source_filename: orion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.orionhealth.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: false\n- host: www.orionhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 17:50:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.orionhealth.com\n  https: false\ndomains:\n- domain: orionhealth.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: orionhealth.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orion/refs/heads/main/security/orion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- EHR
- FHIR
- Health IT
- Healthcare
- HIE
- HL7
- Integration
- Interoperability
- Population Health
---
