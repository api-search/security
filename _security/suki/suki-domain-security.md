---
api_specs:
- filename: suki-ambient-api-openapi.yml
  format: yaml
  label: Suki Ambient API
  slug: suki-ambient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suki/refs/heads/main/openapi/suki-ambient-api-openapi.yml
- filename: suki-dictation-api-openapi.yml
  format: yaml
  label: Suki Dictation API
  slug: suki-dictation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suki/refs/heads/main/openapi/suki-dictation-api-openapi.yml
- filename: suki-form-filling-api-openapi.yml
  format: yaml
  label: Suki Form Filling API
  slug: suki-form-filling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suki/refs/heads/main/openapi/suki-form-filling-api-openapi.yml
- filename: suki-auth-api-openapi.yml
  format: yaml
  label: Suki Auth API
  slug: suki-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suki/refs/heads/main/openapi/suki-auth-api-openapi.yml
- filename: suki-info-api-openapi.yml
  format: yaml
  label: Suki Info API
  slug: suki-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suki/refs/heads/main/openapi/suki-info-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "ssl.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: suki.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: suki-stage.com
  spf: false
hosts:
- cert_expires: Sep 21 04:42:37 2026 GMT
  host: www.suki.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 11:21:10 2026 GMT
  host: developer.suki.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: sdp.suki-stage.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Suki Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Suki AI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Suki AI
provider_slug: suki
slug: suki-domain-security
source_filename: suki-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.suki.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 04:42:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.suki.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 11:21:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: sdp.suki-stage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: suki.ai\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: suki-stage.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suki/refs/heads/main/security/suki-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Artificial Intelligence
- Ambient Clinical Intelligence
- Medical Scribe
- Clinical Documentation
- Voice AI
- Speech Recognition
- Healthcare
- EHR Integration
- Epic
- Oracle Health
- athenahealth
- MEDITECH
- Dictation
- Form Filling
- Note Generation
- Generative AI
- HIPAA
- SOC2
- Healthcare Technology
---
