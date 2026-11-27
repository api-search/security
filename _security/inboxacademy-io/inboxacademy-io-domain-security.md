---
api_specs:
- filename: inboxacademy-io-learning-api-openapi.yml
  format: yaml
  label: Inbox Academy Learning API
  slug: inboxacademy-io-learning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxacademy-io/openapi/inboxacademy-io-learning-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: inboxacademy.io
  spf: false
hosts:
- cert_expires: Feb  4 17:02:17 2027 GMT
  host: inboxacademy.io
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Inbox Academy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inbox Academy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Inbox Academy
provider_slug: inboxacademy-io
slug: inboxacademy-io-domain-security
source_filename: inboxacademy-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inboxacademy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 17:02:17 2027 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: inboxacademy.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/inboxacademy-io/security/inboxacademy-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- Onboarding
- Training
- Education
- Software-as-a-Service
- Platform
---
