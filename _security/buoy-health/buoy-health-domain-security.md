---
api_specs:
- filename: buoy-health-complaints-api-openapi.yml
  format: yaml
  label: Buoy Health Complaints API
  slug: buoy-health-complaints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buoy-health/refs/heads/main/openapi/buoy-health-complaints-api-openapi.yml
- filename: buoy-health-intents-api-openapi.yml
  format: yaml
  label: Buoy Health Intents API
  slug: buoy-health-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buoy-health/refs/heads/main/openapi/buoy-health-intents-api-openapi.yml
- filename: buoy-health-interviews-api-openapi.yml
  format: yaml
  label: Buoy Health Interviews API
  slug: buoy-health-interviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buoy-health/refs/heads/main/openapi/buoy-health-interviews-api-openapi.yml
- filename: buoy-health-queries-api-openapi.yml
  format: yaml
  label: Buoy Health Queries API
  slug: buoy-health-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buoy-health/refs/heads/main/openapi/buoy-health-queries-api-openapi.yml
- filename: buoy-health-questions-api-openapi.yml
  format: yaml
  label: Buoy Health Questions API
  slug: buoy-health-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buoy-health/refs/heads/main/openapi/buoy-health-questions-api-openapi.yml
- filename: buoy-health-results-api-openapi.yml
  format: yaml
  label: Buoy Health Results API
  slug: buoy-health-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buoy-health/refs/heads/main/openapi/buoy-health-results-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: buoyhealth.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: www.buoyhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: buoyhealth.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: api.buoyhealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Buoy Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buoy Health, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Buoy Health
provider_slug: buoy-health
slug: buoy-health-domain-security
source_filename: buoy-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.buoyhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: false\n- host: buoyhealth.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.buoyhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: buoyhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buoy-health/refs/heads/main/security/buoy-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Symptom Checker
- medical-triage
- Digital Health
- Healthcare
- Clinical AI
- Care Navigation
- Patient Engagement
- Diagnosis
- Telehealth
- Authentication
---
