---
api_specs:
- filename: canvas-lms-rest-api-openapi.yml
  format: yaml
  label: Canvas REST API
  slug: canvas-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canvas-lms/refs/heads/main/openapi/canvas-lms-rest-api-openapi.yml
- filename: canvas-lms-live-events-asyncapi.yml
  format: yaml
  label: Canvas Live Events
  slug: canvas-live-events
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/canvas-lms/refs/heads/main/openapi/canvas-lms-live-events-asyncapi.yml
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
