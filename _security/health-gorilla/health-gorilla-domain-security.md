---
api_specs:
- filename: health-gorilla-openapi.yml
  format: yaml
  label: Patients (FHIR)
  slug: patients-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-openapi.yml
- filename: health-gorilla-openapi.yml
  format: yaml
  label: Record Query/Retrieval
  slug: record-query
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-openapi.yml
- filename: health-gorilla-openapi.yml
  format: yaml
  label: Lab Ordering
  slug: lab-ordering
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-openapi.yml
- filename: health-gorilla-openapi.yml
  format: yaml
  label: Diagnostic Reports
  slug: diagnostic-reports
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-openapi.yml
- filename: health-gorilla-openapi.yml
  format: yaml
  label: Documents
  slug: documents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-openapi.yml
- filename: health-gorilla-openapi.yml
  format: yaml
  label: Eligibility
  slug: eligibility
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: healthgorilla.com
  spf: true
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: www.healthgorilla.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 20:33:21 2026 GMT
  host: developer.healthgorilla.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: api.healthgorilla.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Health Gorilla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Health Gorilla, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Health Gorilla
provider_slug: health-gorilla
slug: health-gorilla-domain-security
source_filename: health-gorilla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.healthgorilla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.healthgorilla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:33:21 2026 GMT\n  hsts: null\n- host: api.healthgorilla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: healthgorilla.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/security/health-gorilla-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- Interoperability
- FHIR
- Clinical Data
- Lab Ordering
---
