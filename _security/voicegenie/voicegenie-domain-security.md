---
api_specs:
- filename: voicegenie-openapi.yml
  format: yaml
  label: VoiceGenie Public REST API
  slug: voicegenie-public-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voicegenie/refs/heads/main/openapi/voicegenie-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: voicegenie.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gitbook.io
  spf: true
hosts:
- cert_expires: Oct 18 23:03:49 2026 GMT
  host: voicegenie.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 19:03:12 2026 GMT
  host: voicegenie.gitbook.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: core-saas.voicegenie.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Voicegenie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VoiceGenie, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: VoiceGenie
provider_slug: voicegenie
slug: voicegenie-domain-security
source_filename: voicegenie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: voicegenie.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:03:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: voicegenie.gitbook.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 19:03:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: core-saas.voicegenie.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: voicegenie.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: gitbook.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voicegenie/refs/heads/main/security/voicegenie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Voice AI
- Conversational AI
- Sales Automation
- Voice Agents
- Telephony
- Call Center
- Customer Support
- Lead Generation
- Webhooks
---
