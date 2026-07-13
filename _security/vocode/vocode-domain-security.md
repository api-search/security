---
api_specs:
- filename: vocode-openapi.yml
  format: yaml
  label: Vocode Calls API
  slug: vocode-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vocode/refs/heads/main/openapi/vocode-openapi.yml
- filename: vocode-openapi.yml
  format: yaml
  label: Vocode Agents API
  slug: vocode-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vocode/refs/heads/main/openapi/vocode-openapi.yml
- filename: vocode-openapi.yml
  format: yaml
  label: Vocode Phone Numbers API
  slug: vocode-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vocode/refs/heads/main/openapi/vocode-openapi.yml
- filename: vocode-openapi.yml
  format: yaml
  label: Vocode Actions API
  slug: vocode-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vocode/refs/heads/main/openapi/vocode-openapi.yml
- filename: vocode-openapi.yml
  format: yaml
  label: Vocode Voices API
  slug: vocode-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vocode/refs/heads/main/openapi/vocode-openapi.yml
- filename: vocode-openapi.yml
  format: yaml
  label: Vocode Webhooks API
  slug: vocode-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vocode/refs/heads/main/openapi/vocode-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vocode.dev
  spf: true
hosts:
- cert_expires: Sep 15 07:58:20 2026 GMT
  host: www.vocode.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 14:35:54 2026 GMT
  host: docs.vocode.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.vocode.dev
  https: false
kind: domain-security
layout: security
method: probed
name: Vocode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vocode, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vocode
provider_slug: vocode
slug: vocode-domain-security
source_filename: vocode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vocode.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 07:58:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.vocode.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 14:35:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.vocode.dev\n  https: false\ndomains:\n- domain: vocode.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vocode/refs/heads/main/security/vocode-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Voice AI
- Voice Agents
- Telephony
- Conversational AI
- Phone Calls
---
