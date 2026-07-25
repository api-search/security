---
api_specs:
- filename: canvas-lms-live-events-asyncapi.yml
  format: yaml
  label: Canvas Live Events
  slug: canvas-live-events
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/canvas-lms/refs/heads/main/openapi/canvas-lms-live-events-asyncapi.yml
- filename: canvas-lms-accounts-api-openapi.yml
  format: yaml
  label: Canvas LMS Accounts API
  slug: canvas-lms-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canvas-lms/refs/heads/main/openapi/canvas-lms-accounts-api-openapi.yml
- filename: canvas-lms-assignments-api-openapi.yml
  format: yaml
  label: Canvas LMS Assignments API
  slug: canvas-lms-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canvas-lms/refs/heads/main/openapi/canvas-lms-assignments-api-openapi.yml
- filename: canvas-lms-courses-api-openapi.yml
  format: yaml
  label: Canvas LMS Courses API
  slug: canvas-lms-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canvas-lms/refs/heads/main/openapi/canvas-lms-courses-api-openapi.yml
- filename: canvas-lms-discussions-api-openapi.yml
  format: yaml
  label: Canvas LMS Discussions API
  slug: canvas-lms-discussions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canvas-lms/refs/heads/main/openapi/canvas-lms-discussions-api-openapi.yml
- filename: canvas-lms-enrollments-api-openapi.yml
  format: yaml
  label: Canvas LMS Enrollments API
  slug: canvas-lms-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canvas-lms/refs/heads/main/openapi/canvas-lms-enrollments-api-openapi.yml
- filename: canvas-lms-files-api-openapi.yml
  format: yaml
  label: Canvas LMS Files API
  slug: canvas-lms-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canvas-lms/refs/heads/main/openapi/canvas-lms-files-api-openapi.yml
- filename: canvas-lms-modules-api-openapi.yml
  format: yaml
  label: Canvas LMS Modules API
  slug: canvas-lms-modules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canvas-lms/refs/heads/main/openapi/canvas-lms-modules-api-openapi.yml
- filename: canvas-lms-outcomes-api-openapi.yml
  format: yaml
  label: Canvas LMS Outcomes API
  slug: canvas-lms-outcomes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canvas-lms/refs/heads/main/openapi/canvas-lms-outcomes-api-openapi.yml
- filename: canvas-lms-submissions-api-openapi.yml
  format: yaml
  label: Canvas LMS Submissions API
  slug: canvas-lms-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canvas-lms/refs/heads/main/openapi/canvas-lms-submissions-api-openapi.yml
- filename: canvas-lms-users-api-openapi.yml
  format: yaml
  label: Canvas LMS Users API
  slug: canvas-lms-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canvas-lms/refs/heads/main/openapi/canvas-lms-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: instructure.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Aug  4 02:52:44 2026 GMT
  host: www.instructure.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: canvas.instructure.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: data-access-platform-api.s3.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Canvas Lms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canvas LMS, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Canvas LMS
provider_slug: canvas-lms
slug: canvas-lms-domain-security
source_filename: canvas-lms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.instructure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 02:52:44 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: canvas.instructure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: null\n- host: data-access-platform-api.s3.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: instructure.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canvas-lms/refs/heads/main/security/canvas-lms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Learning Management
- Education
- EdTech
- LMS
- LTI
- Higher Education
- K-12
- Open Source
- AGPL
- Canvas
---
