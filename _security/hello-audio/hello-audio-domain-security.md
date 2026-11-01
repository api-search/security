---
api_specs:
- filename: hello-audio-hello-audio-api-api-openapi.yml
  format: yaml
  label: Hello Audio API
  slug: hello-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hello-audio/openapi/hello-audio-hello-audio-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: helloaudio.fm
  spf: true
hosts:
- cert_expires: Apr 30 23:59:59 2027 GMT
  host: helloaudio.fm
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 05:12:57 2026 GMT
  host: help.helloaudio.fm
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Hello Audio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hello Audio, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hello Audio
provider_slug: hello-audio
slug: hello-audio-domain-security
source_filename: hello-audio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: helloaudio.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 30 23:59:59 2027 GMT\n  hsts: null\n- host: help.helloaudio.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 05:12:57 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: helloaudio.fm\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hello-audio/security/hello-audio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Audio
- Podcast
- SaaS
- Private
- Private Podcasts
- Webhooks
- Zapier
- Creator Economy
---
