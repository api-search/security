---
api_specs:
- filename: email-verifier-api-openapi.yml
  format: yaml
  label: Email Verifier API Verification
  slug: verification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/email-verifier-api/refs/heads/main/openapi/email-verifier-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: emailverifierapi.com
  spf: false
hosts:
- cert_expires: Oct  8 18:38:37 2026 GMT
  host: emailverifierapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Email Verifier Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Email Verifier API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Email Verifier API
provider_slug: email-verifier-api
slug: email-verifier-api-domain-security
source_filename: email-verifier-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emailverifierapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 18:38:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: emailverifierapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/email-verifier-api/refs/heads/main/security/email-verifier-api-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Email Verification
- Deliverability
- SMTP Check
- Bounce Prevention
- Lead Validation
- Disposable Detection
- Spam Trap Detection
- Catch-All Detection
- Greylisting
- Role Account Detection
- Typo Suggestion
- B2B Lead Scoring
---
