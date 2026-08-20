---
api_specs:
- filename: heidi-health-ask-heidi-api-openapi.yml
  format: yaml
  label: Heidi Health Ask Heidi API
  slug: heidi-health-ask-heidi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-ask-heidi-api-openapi.yml
- filename: heidi-health-authentication-api-openapi.yml
  format: yaml
  label: Heidi Health Authentication API
  slug: heidi-health-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-authentication-api-openapi.yml
- filename: heidi-health-clinical-coding-api-openapi.yml
  format: yaml
  label: Heidi Health Clinical Coding API
  slug: heidi-health-clinical-coding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-clinical-coding-api-openapi.yml
- filename: heidi-health-consult-notes-api-openapi.yml
  format: yaml
  label: Heidi Health Consult Notes API
  slug: heidi-health-consult-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-consult-notes-api-openapi.yml
- filename: heidi-health-documents-api-openapi.yml
  format: yaml
  label: Heidi Health Documents API
  slug: heidi-health-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-documents-api-openapi.yml
- filename: heidi-health-patient-profiles-api-openapi.yml
  format: yaml
  label: Heidi Health Patient Profiles API
  slug: heidi-health-patient-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-patient-profiles-api-openapi.yml
- filename: heidi-health-session-context-api-openapi.yml
  format: yaml
  label: Heidi Health Session Context API
  slug: heidi-health-session-context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-session-context-api-openapi.yml
- filename: heidi-health-sessions-api-openapi.yml
  format: yaml
  label: Heidi Health Sessions API
  slug: heidi-health-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-sessions-api-openapi.yml
- filename: heidi-health-templates-api-openapi.yml
  format: yaml
  label: Heidi Health Templates API
  slug: heidi-health-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-templates-api-openapi.yml
- filename: heidi-health-transcription-api-openapi.yml
  format: yaml
  label: Heidi Health Transcription API
  slug: heidi-health-transcription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-transcription-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: heidihealth.com
  spf: true
hosts:
- cert_expires: Sep 11 07:09:17 2026 GMT
  host: www.heidihealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: registrar.api.heidihealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Heidi Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heidi Health, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Heidi Health
provider_slug: heidi-health
slug: heidi-health-domain-security
source_filename: heidi-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.heidihealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 07:09:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: registrar.api.heidihealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: heidihealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/security/heidi-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Health Tech
- AI Medical Scribe
- Ambient AI
- Clinical Documentation
- Clinical Decision Support
- Artificial Intelligence
- Speech-to-Text
- Transcription
- EHR Integration
- Electronic Health Records
- Telehealth
- Clinical Coding
- ICD-10
- SNOMED
- HIPAA
- GDPR
- SOC 2
- ISO 27001
- ISO 42001
- Wearables
- Voice
- Audio
- Australia
- Melbourne
---
