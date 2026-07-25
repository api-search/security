---
api_specs:
- filename: gp-connect-appointment-api-openapi.yml
  format: yaml
  label: GP Connect Appointment API
  slug: gp-connect-appointment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gp-connect/refs/heads/main/openapi/gp-connect-appointment-api-openapi.yml
- filename: gp-connect-documents-api-openapi.yml
  format: yaml
  label: GP Connect Documents API
  slug: gp-connect-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gp-connect/refs/heads/main/openapi/gp-connect-documents-api-openapi.yml
- filename: gp-connect-fhir-api-openapi.yml
  format: yaml
  label: GP Connect FHIR API
  slug: gp-connect-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gp-connect/refs/heads/main/openapi/gp-connect-fhir-api-openapi.yml
- filename: gp-connect-meta-api-openapi.yml
  format: yaml
  label: GP Connect Meta API
  slug: gp-connect-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gp-connect/refs/heads/main/openapi/gp-connect-meta-api-openapi.yml
- filename: gp-connect-patient-api-openapi.yml
  format: yaml
  label: GP Connect Patient API
  slug: gp-connect-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gp-connect/refs/heads/main/openapi/gp-connect-patient-api-openapi.yml
- filename: gp-connect-slot-api-openapi.yml
  format: yaml
  label: GP Connect Slot API
  slug: gp-connect-slot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gp-connect/refs/heads/main/openapi/gp-connect-slot-api-openapi.yml
- filename: gp-connect-task-api-openapi.yml
  format: yaml
  label: GP Connect Task API
  slug: gp-connect-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gp-connect/refs/heads/main/openapi/gp-connect-task-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nhs.uk
  spf: true
hosts:
- cert_expires: Sep 24 21:58:44 2026 GMT
  host: digital.nhs.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: sandbox.api.service.nhs.uk
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: int.api.service.nhs.uk
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Gp Connect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GP Connect, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GP Connect
provider_slug: gp-connect
slug: gp-connect-domain-security
source_filename: gp-connect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: digital.nhs.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 21:58:44 2026 GMT\n  hsts: null\n- host: sandbox.api.service.nhs.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: null\n- host: int.api.service.nhs.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: nhs.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gp-connect/refs/heads/main/security/gp-connect-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- NHS
- FHIR
- Healthcare
- GP Records
- Appointments
- Prescriptions
- Interoperability
- UK
- Patient Records
- Electronic Health Records
- FHIR STU3
- FHIR R4
---
