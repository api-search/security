---
api_specs:
- filename: suki-ai-openapi.yml
  format: yaml
  label: Suki Platform REST API
  slug: suki-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suki-ai/refs/heads/main/openapi/suki-ai-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "ssl.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: suki.ai
  spf: true
hosts:
- cert_expires: Sep 21 04:42:37 2026 GMT
  host: www.suki.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 11:21:10 2026 GMT
  host: developer.suki.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Suki Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Suki AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Suki AI
provider_slug: suki-ai
slug: suki-ai-domain-security
source_filename: suki-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.suki.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 04:42:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.suki.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 11:21:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: suki.ai\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suki-ai/refs/heads/main/security/suki-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- Ambient AI
- Clinical Documentation
- Voice AI
- Speech Recognition
- EHR Integration
- SDK
- Dictation
---
