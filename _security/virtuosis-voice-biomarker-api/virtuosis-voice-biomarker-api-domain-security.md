---
api_specs:
- filename: virtuosis-voice-biomarker-api-accounts-api-openapi.yml
  format: yaml
  label: Virtuosis Voice Biomarker API Accounts API
  slug: virtuosis-voice-biomarker-api-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuosis-voice-biomarker-api/refs/heads/main/openapi/virtuosis-voice-biomarker-api-accounts-api-openapi.yml
- filename: virtuosis-voice-biomarker-api-default-api-openapi.yml
  format: yaml
  label: Virtuosis Voice Biomarker API Voice Biomarker Api Default API
  slug: virtuosis-voice-biomarker-api-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuosis-voice-biomarker-api/refs/heads/main/openapi/virtuosis-voice-biomarker-api-default-api-openapi.yml
- filename: virtuosis-voice-biomarker-api-recordings-api-openapi.yml
  format: yaml
  label: Virtuosis Voice Biomarker API Recordings API
  slug: virtuosis-voice-biomarker-api-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuosis-voice-biomarker-api/refs/heads/main/openapi/virtuosis-voice-biomarker-api-recordings-api-openapi.yml
- filename: virtuosis-voice-biomarker-api-usage-api-openapi.yml
  format: yaml
  label: Virtuosis Voice Biomarker API Usage API
  slug: virtuosis-voice-biomarker-api-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuosis-voice-biomarker-api/refs/heads/main/openapi/virtuosis-voice-biomarker-api-usage-api-openapi.yml
- filename: api-reference.yaml
  format: yaml
  label: Virtuosis Voice Biomarker API
  slug: virtuosis-voice-biomarker-api
  spec_type: OpenAPI
  url: https://docs.virtuosis.ai/openapi/api-reference.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: virtuosis.ai
  spf: true
hosts:
- cert_expires: Oct 16 03:24:27 2026 GMT
  host: docs.virtuosis.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: api.virtuosis.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Virtuosis Voice Biomarker Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virtuosis Voice Biomarker API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Virtuosis Voice Biomarker API
provider_slug: virtuosis-voice-biomarker-api
slug: virtuosis-voice-biomarker-api-domain-security
source_filename: virtuosis-voice-biomarker-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.virtuosis.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 03:24:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.virtuosis.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: virtuosis.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtuosis-voice-biomarker-api/refs/heads/main/security/virtuosis-voice-biomarker-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Health
- voice biomarkers
- speech analysis
- acoustic analysis
- Medical Device
- Mental Health
- Wellbeing
- neurodegenerative screening
- Telehealth
- Remote Monitoring
- communication coaching
- Clinical Research
- Health AI
- Clinical Decision Support
---
