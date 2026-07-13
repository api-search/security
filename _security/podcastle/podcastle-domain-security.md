---
api_specs:
- filename: podcastle-openapi.yml
  format: yaml
  label: Podcastle Text-to-Speech API
  slug: text-to-speech
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastle/refs/heads/main/openapi/podcastle-openapi.yml
- filename: podcastle-openapi.yml
  format: yaml
  label: Podcastle Voices API
  slug: voices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastle/refs/heads/main/openapi/podcastle-openapi.yml
- filename: podcastle-openapi.yml
  format: yaml
  label: Podcastle Voice Cloning API
  slug: voice-cloning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastle/refs/heads/main/openapi/podcastle-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: podcastle.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: async.com
  spf: true
hosts:
- cert_expires: Sep  6 22:15:43 2026 GMT
  host: podcastle.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 00:03:30 2026 GMT
  host: docs.async.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: api.async.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Podcastle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Podcastle, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Podcastle
provider_slug: podcastle
slug: podcastle-domain-security
source_filename: podcastle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: podcastle.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 22:15:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.async.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  9 00:03:30 2026 GMT\n  hsts: false\n- host: api.async.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: podcastle.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: async.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/podcastle/refs/heads/main/security/podcastle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Audio
- Text to Speech
- Voice Cloning
- Podcasting
---
