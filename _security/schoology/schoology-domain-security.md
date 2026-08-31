---
api_specs:
- filename: schoology-assignments-api-openapi.yml
  format: yaml
  label: Schoology Assignments API
  slug: schoology-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-assignments-api-openapi.yml
- filename: schoology-courses-api-openapi.yml
  format: yaml
  label: Schoology Courses API
  slug: schoology-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-courses-api-openapi.yml
- filename: schoology-enrollments-api-openapi.yml
  format: yaml
  label: Schoology Enrollments API
  slug: schoology-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-enrollments-api-openapi.yml
- filename: schoology-grades-api-openapi.yml
  format: yaml
  label: Schoology Grades API
  slug: schoology-grades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-grades-api-openapi.yml
- filename: schoology-groups-api-openapi.yml
  format: yaml
  label: Schoology Groups API
  slug: schoology-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-groups-api-openapi.yml
- filename: schoology-multi-call-api-openapi.yml
  format: yaml
  label: Schoology Multi-Call API
  slug: schoology-multi-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-multi-call-api-openapi.yml
- filename: schoology-sections-api-openapi.yml
  format: yaml
  label: Schoology Sections API
  slug: schoology-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-sections-api-openapi.yml
- filename: schoology-submissions-api-openapi.yml
  format: yaml
  label: Schoology Submissions API
  slug: schoology-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-submissions-api-openapi.yml
- filename: schoology-subscriptions-api-openapi.yml
  format: yaml
  label: Schoology Subscriptions API
  slug: schoology-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-subscriptions-api-openapi.yml
- filename: schoology-targets-api-openapi.yml
  format: yaml
  label: Schoology Targets API
  slug: schoology-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-targets-api-openapi.yml
- filename: schoology-users-api-openapi.yml
  format: yaml
  label: Schoology Users API
  slug: schoology-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-users-api-openapi.yml
- filename: schoology-events-api-openapi.yml
  format: yaml
  label: Schoology Events API
  slug: schoology-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-events-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: schoology.com
  spf: true
hosts:
- cert_expires: Aug  4 00:22:56 2026 GMT
  host: www.schoology.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: developers.schoology.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: api.schoology.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Schoology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Schoology, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Schoology
provider_slug: schoology
slug: schoology-domain-security
source_filename: schoology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.schoology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 00:22:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.schoology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: false\n- host: api.schoology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: schoology.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/security/schoology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- EdTech
- LMS
- K-12
---
