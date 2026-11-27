---
api_specs:
- filename: aicertificates-study-content-api-openapi.yml
  format: yaml
  label: AI Certificates Content API
  slug: aicertificates-study-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicertificates-study/openapi/aicertificates-study-content-api-openapi.yml
- filename: aicertificates-study-readiness-api-openapi.yml
  format: yaml
  label: AI Certificates Readiness API
  slug: aicertificates-study-readiness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicertificates-study/openapi/aicertificates-study-readiness-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: aicertificates.study
  spf: false
hosts:
- cert_expires: Jan 22 23:44:53 2027 GMT
  host: aicertificates.study
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AI Certificates Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Certificates, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AI Certificates
provider_slug: aicertificates-study
slug: aicertificates-study-domain-security
source_filename: aicertificates-study-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aicertificates.study\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:44:53 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aicertificates.study\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/aicertificates-study/security/aicertificates-study-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Education
- Artificial Intelligence
- Certification
- Practice Exams
- Anthropic
---
