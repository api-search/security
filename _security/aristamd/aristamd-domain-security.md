---
api_specs:
- filename: aristamd-comments-api-openapi.yml
  format: yaml
  label: AristaMD Comments API
  slug: aristamd-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-comments-api-openapi.yml
- filename: aristamd-diagnostic-api-openapi.yml
  format: yaml
  label: AristaMD Diagnostic API
  slug: aristamd-diagnostic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-diagnostic-api-openapi.yml
- filename: aristamd-econsults-api-openapi.yml
  format: yaml
  label: AristaMD E Consults API
  slug: aristamd-econsults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-econsults-api-openapi.yml
- filename: aristamd-intergy-patients-api-openapi.yml
  format: yaml
  label: AristaMD Intergy/Patients API
  slug: aristamd-intergy-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-intergy-patients-api-openapi.yml
- filename: aristamd-panelists-api-openapi.yml
  format: yaml
  label: AristaMD Panelists API
  slug: aristamd-panelists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-panelists-api-openapi.yml
- filename: aristamd-patients-api-openapi.yml
  format: yaml
  label: AristaMD Patients API
  slug: aristamd-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-patients-api-openapi.yml
- filename: aristamd-requests-api-openapi.yml
  format: yaml
  label: AristaMD Requests API
  slug: aristamd-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-requests-api-openapi.yml
- filename: aristamd-reviews-api-openapi.yml
  format: yaml
  label: AristaMD Reviews API
  slug: aristamd-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-reviews-api-openapi.yml
- filename: aristamd-specialties-api-openapi.yml
  format: yaml
  label: AristaMD Specialties API
  slug: aristamd-specialties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-specialties-api-openapi.yml
- filename: aristamd-specialty-api-openapi.yml
  format: yaml
  label: AristaMD Specialty API
  slug: aristamd-specialty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-specialty-api-openapi.yml
- filename: aristamd-users-api-openapi.yml
  format: yaml
  label: AristaMD Users API
  slug: aristamd-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-users-api-openapi.yml
- filename: aristamd-workup-checklists-api-openapi.yml
  format: yaml
  label: AristaMD Workup Checklists API
  slug: aristamd-workup-checklists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-workup-checklists-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aristamd.com
  spf: true
hosts:
- cert_expires: Oct 20 01:23:31 2026 GMT
  host: www.aristamd.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 11:05:20 2026 GMT
  host: api.aristamd.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  note: 'Corrected by hand after the automated probe recorded null. The API host root answers 404 (JSON), which the probe skipped; a direct HEAD of both https://api.aristamd.com/ and https://api.aristamd.com/econsults returns "Strict-Transport-Security: max-age=63072000; includeSubDomains; preload". The marketing host www.aristamd.com sends no HSTS header at all.'
  other_headers:
    access_control_allow_origin: '*'
    referrer_policy: strict-origin-when-cross-origin
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aristamd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AristaMD, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AristaMD
provider_slug: aristamd
slug: aristamd-domain-security
source_filename: aristamd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aristamd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 01:23:31 2026 GMT\n  hsts: false\n- host: api.aristamd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 11:05:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: >-\n    Corrected by hand after the automated probe recorded null. The API host root\n    answers 404 (JSON), which the probe skipped; a direct HEAD of both\n    https://api.aristamd.com/ and https://api.aristamd.com/econsults returns\n    \"Strict-Transport-Security: max-age=63072000; includeSubDomains; preload\".\n    The marketing host www.aristamd.com sends no HSTS header at all.\n  other_headers:\n    referrer_policy: strict-origin-when-cross-origin\n    access_control_allow_origin: '*'\ndomains:\n- domain: aristamd.com\n  dnssec: false\n\
  \  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/security/aristamd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Digital Health
- Telehealth
- eConsult
- Specialty Care
- Referrals
- Care Coordination
- Health Plans
- Medicaid
- HL7
- Electronic Health Records
---
