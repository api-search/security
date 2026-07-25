---
api_specs:
- filename: hibob-attendance-api-openapi.yml
  format: yaml
  label: HiBob Attendance API
  slug: hibob-attendance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hibob/refs/heads/main/openapi/hibob-attendance-api-openapi.yml
- filename: hibob-documents-api-openapi.yml
  format: yaml
  label: HiBob Documents API
  slug: hibob-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hibob/refs/heads/main/openapi/hibob-documents-api-openapi.yml
- filename: hibob-employee-tables-api-openapi.yml
  format: yaml
  label: HiBob Employee Tables API
  slug: hibob-employee-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hibob/refs/heads/main/openapi/hibob-employee-tables-api-openapi.yml
- filename: hibob-goals-api-openapi.yml
  format: yaml
  label: HiBob Goals API
  slug: hibob-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hibob/refs/heads/main/openapi/hibob-goals-api-openapi.yml
- filename: hibob-hiring-api-openapi.yml
  format: yaml
  label: HiBob Hiring API
  slug: hibob-hiring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hibob/refs/heads/main/openapi/hibob-hiring-api-openapi.yml
- filename: hibob-learning-api-openapi.yml
  format: yaml
  label: HiBob Learning API
  slug: hibob-learning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hibob/refs/heads/main/openapi/hibob-learning-api-openapi.yml
- filename: hibob-people-api-openapi.yml
  format: yaml
  label: HiBob People API
  slug: hibob-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hibob/refs/heads/main/openapi/hibob-people-api-openapi.yml
- filename: hibob-projects-api-openapi.yml
  format: yaml
  label: HiBob Projects API
  slug: hibob-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hibob/refs/heads/main/openapi/hibob-projects-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hibob.com
  spf: true
hosts:
- cert_expires: Nov  9 11:27:00 2026 GMT
  host: www.hibob.com
  hsts: true
  hsts_max_age: 6
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 21:36:06 2026 GMT
  host: apidocs.hibob.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 11:05:12 2026 GMT
  host: api.hibob.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hibob Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HiBob, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HiBob
provider_slug: hibob
slug: hibob-domain-security
source_filename: hibob-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hibob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 11:27:00 2026 GMT\n  hsts: true\n  hsts_max_age: 6\n- host: apidocs.hibob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 21:36:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.hibob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 11:05:12 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: hibob.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hibob/refs/heads/main/security/hibob-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HR
- HRIS
- People Operations
- Employee Data
- Time Off
- HR Tech
---
