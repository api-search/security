---
api_specs:
- filename: personal-demographics-service-api
  format: yaml
  label: Personal Demographics Service - FHIR API
  slug: personal-demographics-service-fhir-api
  spec_type: OpenAPI
  url: https://github.com/NHSDigital/personal-demographics-service-api
- filename: gp-connect-access-record-fhir-api
  format: yaml
  label: GP Connect Access Record Structured - FHIR API
  slug: gp-connect-access-record-structured-fhir-api
  spec_type: OpenAPI
  url: https://github.com/NHSDigital/gp-connect-access-record-fhir-api
- filename: gp-connect-appointments-management-fhir
  format: yaml
  label: GP Connect Appointment Management - FHIR API
  slug: gp-connect-appointment-management-fhir-api
  spec_type: OpenAPI
  url: https://github.com/NHSDigital/gp-connect-appointments-management-fhir
- filename: electronic-prescription-service-api
  format: yaml
  label: Electronic Prescription Service - FHIR API
  slug: electronic-prescription-service-fhir-api
  spec_type: OpenAPI
  url: https://github.com/NHSDigital/electronic-prescription-service-api
- filename: openapi.yaml
  format: yaml
  label: NHS Login API
  slug: nhs-login-api
  spec_type: OpenAPI
  url: https://nhsconnect.github.io/nhslogin/scopes-and-claims/
- filename: organisation-data-service-fhir-api
  format: yaml
  label: Organisation Data Service - FHIR API
  slug: organisation-data-service-fhir-api
  spec_type: OpenAPI
  url: https://github.com/NHSDigital/organisation-data-service-fhir-api
- filename: spine-directory-service-api
  format: yaml
  label: Spine Directory Service - FHIR API
  slug: spine-directory-service-fhir-api
  spec_type: OpenAPI
  url: https://github.com/NHSDigital/spine-directory-service-api
- filename: e-referrals-service-api
  format: yaml
  label: NHS e-Referral Service - FHIR API
  slug: nhs-e-referral-service-fhir-api
  spec_type: OpenAPI
  url: https://github.com/NHSDigital/e-referrals-service-api
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
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: api.service.nhs.uk
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: auth.login.nhs.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nhs Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NHS API, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NHS API
provider_slug: nhs-api
slug: nhs-api-domain-security
source_filename: nhs-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: digital.nhs.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 21:58:44 2026 GMT\n  hsts: null\n- host: api.service.nhs.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\n- host: auth.login.nhs.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: nhs.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/security/nhs-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- FHIR
- NHS
- UK
- HL7
- Electronic Prescriptions
- Patient Demographics
- GP Connect
- NHS Login
- Interoperability
---
