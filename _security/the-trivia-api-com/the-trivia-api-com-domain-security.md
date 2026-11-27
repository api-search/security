---
api_specs:
- filename: the-trivia-api-com-meta-api-openapi.yml
  format: yaml
  label: The Trivia API Meta API
  slug: the-trivia-api-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/the-trivia-api-com/openapi/the-trivia-api-com-meta-api-openapi.yml
- filename: the-trivia-api-com-questions-api-openapi.yml
  format: yaml
  label: The Trivia API Questions API
  slug: the-trivia-api-com-questions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/the-trivia-api-com/openapi/the-trivia-api-com-questions-api-openapi.yml
- filename: the-trivia-api-com-quizzes-api-openapi.yml
  format: yaml
  label: The Trivia API Quizzes API
  slug: the-trivia-api-com-quizzes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/the-trivia-api-com/openapi/the-trivia-api-com-quizzes-api-openapi.yml
- filename: the-trivia-api-com-sessions-api-openapi.yml
  format: yaml
  label: The Trivia API Sessions API
  slug: the-trivia-api-com-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/the-trivia-api-com/openapi/the-trivia-api-com-sessions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: the-trivia-api.com
  spf: true
hosts:
- cert_expires: Jan 19 20:24:27 2027 GMT
  host: the-trivia-api.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: The Trivia API Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Trivia API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: The Trivia API
provider_slug: the-trivia-api-com
slug: the-trivia-api-com-domain-security
source_filename: the-trivia-api-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: the-trivia-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 20:24:27 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: the-trivia-api.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/the-trivia-api-com/security/the-trivia-api-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Trivia
- JSON
- Questions
---
