---
api_specs:
- filename: micro1-ai-recruiter-openapi.yml
  format: yaml
  label: micro1 Public API
  slug: micro1-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micro1/refs/heads/main/openapi/micro1-ai-recruiter-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: micro1.ai
  spf: true
hosts:
- cert_expires: Sep 29 22:58:36 2026 GMT
  host: www.micro1.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 22:01:48 2026 GMT
  host: ai-recruiter.micro1.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: public.api.micro1.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Micro1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for micro1, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: micro1
provider_slug: micro1
slug: micro1-domain-security
source_filename: micro1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.micro1.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 22:58:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ai-recruiter.micro1.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 22:01:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: public.api.micro1.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: micro1.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/micro1/refs/heads/main/security/micro1-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- recruiting
- hiring
- ai-interviews
- talent-assessment
- candidate-screening
- applicant-tracking
- human-resources
- proctoring
- webhooks
- agent-native
- ai-training-data
---
