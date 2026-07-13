---
api_specs:
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Authentication API
  slug: heidi-api-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Templates API
  slug: heidi-api-templates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Patient Profiles API
  slug: heidi-api-patient-profiles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Sessions API
  slug: heidi-api-sessions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Session Context API
  slug: heidi-api-session-context
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Session Coding API
  slug: heidi-api-session-coding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Transcription API
  slug: heidi-api-transcription
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Consult Notes API
  slug: heidi-api-consult-notes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Documents API
  slug: heidi-api-documents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Ask Heidi API
  slug: heidi-api-ask-heidi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
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
- Speech To Text
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
