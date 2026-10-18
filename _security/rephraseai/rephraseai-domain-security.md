---
api_specs:
- filename: rephraseai-actor-api-openapi.yml
  format: yaml
  label: Rephrase.ai Actor API
  slug: rephraseai-actor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rephraseai/refs/heads/main/openapi/rephraseai-actor-api-openapi.yml
- filename: rephraseai-authentication-api-openapi.yml
  format: yaml
  label: Rephrase.ai Authentication API
  slug: rephraseai-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rephraseai/refs/heads/main/openapi/rephraseai-authentication-api-openapi.yml
- filename: rephraseai-video-api-openapi.yml
  format: yaml
  label: Rephrase.ai Video API
  slug: rephraseai-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rephraseai/refs/heads/main/openapi/rephraseai-video-api-openapi.yml
- filename: rephraseai-voice-api-openapi.yml
  format: yaml
  label: Rephrase.ai Voice API
  slug: rephraseai-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rephraseai/refs/heads/main/openapi/rephraseai-voice-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: rephrase.ai
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- host: rephrase.ai
  https: false
- cert_expires: Dec  7 17:48:12 2026 GMT
  host: studio-rephrase-api.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: auth.rephrase.ai
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Rephraseai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rephrase.ai, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Rephrase.ai
provider_slug: rephraseai
slug: rephraseai-domain-security
source_filename: rephraseai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rephrase.ai\n  https: false\n- host: studio-rephrase-api.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 17:48:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: auth.rephrase.ai\n  https: false\ndomains:\n- domain: rephrase.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rephraseai/refs/heads/main/security/rephraseai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Generative AI
- Video
- Video Generation
- Avatars
- Media
- Content Creation
---
