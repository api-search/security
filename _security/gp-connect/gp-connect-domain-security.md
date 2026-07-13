---
api_specs:
- filename: gp-connect-access-record-structured-fhir.yaml
  format: yaml
  label: GP Connect Access Record - Structured FHIR API
  slug: access-record-structured-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/NHSDigital/gp-connect-access-record-structured-fhir/master/specification/gp-connect-access-record-structured-fhir.yaml
- filename: gp-connect-appointments-management-fhir.yaml
  format: yaml
  label: GP Connect Appointment Management FHIR API
  slug: appointment-management-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/NHSDigital/gp-connect-appointments-management-fhir/master/specification/gp-connect-appointments-management-fhir.yaml
- filename: gp-connect-update-record-fhir.yaml
  format: yaml
  label: GP Connect Update Record FHIR API
  slug: update-record-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/NHSDigital/gp-connect-update-record-fhir/master/specification/gp-connect-update-record-fhir.yaml
- filename: gp-connect-access-record-fhir.yaml
  format: yaml
  label: GP Connect Patient Facing Access Record FHIR API
  slug: patient-facing-access-record-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/NHSDigital/gp-connect-access-record-fhir/master/specification/gp-connect-access-record-fhir.yaml
- filename: gp-connect-appointments-management-fhir.yaml
  format: yaml
  label: GP Connect Patient Facing Appointment Management FHIR API
  slug: patient-facing-appointments-management-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/NHSDigital/gp-connect-appointments-management-fhir/master/specification/gp-connect-appointments-management-fhir.yaml
- filename: gp-connect-prescriptions-management-fhir.yaml
  format: yaml
  label: GP Connect Patient Facing Prescriptions Management FHIR API
  slug: patient-facing-prescriptions-management-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/NHSDigital/gp-connect-prescriptions-management-fhir/master/specification/gp-connect-prescriptions-management-fhir.yaml
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
