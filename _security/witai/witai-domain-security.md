---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; account=271b0beda0771d006aa3a6c11b05187d456d6c239b46cb5241196095b09c92af"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wit.ai
  spf: true
hosts:
- cert_expires: Jul 29 23:59:59 2026 GMT
  host: wit.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 29 23:59:59 2026 GMT
  host: api.wit.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Witai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wit.AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wit.AI
provider_slug: witai
slug: witai-domain-security
source_filename: witai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wit.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.wit.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: wit.ai\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; account=271b0beda0771d006aa3a6c11b05187d456d6c239b46cb5241196095b09c92af\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/witai/refs/heads/main/security/witai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Natural Language Processing
- NLP
- Speech Recognition
- Speech to Text
- Text to Speech
- Intents
- Entities
- Voice
- Conversational AI
- Machine Learning
- Meta
---
