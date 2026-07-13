---
api_specs:
- filename: openapi.json
  format: json
  label: QuizAPI
  slug: quiz-api
  spec_type: OpenAPI
  url: https://quizapi.io/api/v1/openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: quizapi.io
  spf: true
hosts:
- cert_expires: Sep  9 22:52:49 2026 GMT
  host: quizapi.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quiz Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QuizAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: QuizAPI
provider_slug: quiz-api
slug: quiz-api-domain-security
source_filename: quiz-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quizapi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 22:52:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: quizapi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quiz-api/refs/heads/main/security/quiz-api-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Quizzes
- Trivia
- Education
- Assessment
- Content
---
