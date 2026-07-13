---
api_specs:
- filename: particle-health-openapi.yml
  format: yaml
  label: Particle Health API
  slug: patient-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-health/refs/heads/main/openapi/particle-health-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: particlehealth.com
  spf: true
hosts:
- cert_expires: Oct  8 20:18:24 2026 GMT
  host: particlehealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 21:26:57 2026 GMT
  host: docs.particlehealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 13:24:54 2026 GMT
  host: api.particlehealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Particle Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Particle Health, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Particle Health
provider_slug: particle-health
slug: particle-health-domain-security
source_filename: particle-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: particlehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 20:18:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.particlehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 21:26:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.particlehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 13:24:54 2026 GMT\n  hsts: null\ndomains:\n- domain: particlehealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/particle-health/refs/heads/main/security/particle-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ADT
- C-CDA
- Care Coordination
- Carequality
- Clinical Data
- CommonWell
- Deltas
- eHealth Exchange
- EHR
- FHIR
- Health Data
- Health Information Exchange
- Healthcare
- HIE
- HL7
- HL7v2
- Interoperability
- Medical Records
- Patients
- Pharmacy
- QHIN
- Surescripts
- TEFCA
- USCDI
---
