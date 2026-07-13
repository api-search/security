---
api_specs:
- filename: lovo-ai-openapi.yml
  format: yaml
  label: LOVO AI Text-to-Speech API
  slug: lovo-ai-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lovo-ai/refs/heads/main/openapi/lovo-ai-openapi.yml
- filename: lovo-ai-openapi.yml
  format: yaml
  label: LOVO AI Speakers API
  slug: lovo-ai-speakers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lovo-ai/refs/heads/main/openapi/lovo-ai-openapi.yml
- filename: lovo-ai-openapi.yml
  format: yaml
  label: LOVO AI Pronunciation and Prosody
  slug: lovo-ai-pronunciation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lovo-ai/refs/heads/main/openapi/lovo-ai-openapi.yml
- filename: lovo-ai-openapi.yml
  format: yaml
  label: LOVO AI Teams and Billing API
  slug: lovo-ai-teams-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lovo-ai/refs/heads/main/openapi/lovo-ai-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lovo.ai
  spf: true
hosts:
- cert_expires: Sep  9 21:12:53 2026 GMT
  host: lovo.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 09:26:42 2026 GMT
  host: docs.genny.lovo.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.genny.lovo.ai
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Lovo Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LOVO AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LOVO AI
provider_slug: lovo-ai
slug: lovo-ai-domain-security
source_filename: lovo-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lovo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 21:12:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.genny.lovo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 09:26:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.genny.lovo.ai\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: lovo.ai\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lovo-ai/refs/heads/main/security/lovo-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Text to Speech
- TTS
- Voice Generation
- Voice Cloning
- Speech Synthesis
- Voiceover
---
