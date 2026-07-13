---
api_specs:
- filename: canvas.openapi.yaml
  format: yaml
  label: Canvas LMS REST API
  slug: canvas-lms-rest-api
  spec_type: OpenAPI
  url: https://github.com/instructure/canvas-lms/blob/master/public/doc/openapi/canvas.openapi.yaml
- filename: instructure-canvas-lti-openapi.yml
  format: yaml
  label: Canvas LTI 1.3 API
  slug: canvas-lti-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-canvas-lti-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: instructure.com
  spf: true
hosts:
- cert_expires: Aug  4 02:52:44 2026 GMT
  host: www.instructure.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 09:17:42 2026 GMT
  host: developerdocs.instructure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: api-gateway.instructure.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Instructure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instructure, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Instructure
provider_slug: instructure
slug: instructure-domain-security
source_filename: instructure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.instructure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 02:52:44 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: developerdocs.instructure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 09:17:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-gateway.instructure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: instructure.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/security/instructure-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- EdTech
- Education
- LMS
- Canvas
- Courses
- Enrollments
- Assignments
- Grades
- Discussions
- GraphQL
- LTI
- Learning Management
---
