---
api_specs:
- filename: respeecher-openapi.yml
  format: yaml
  label: Respeecher Voices API
  slug: respeecher-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-openapi.yml
- filename: respeecher-openapi.yml
  format: yaml
  label: Respeecher Speech-to-Speech Conversion API
  slug: respeecher-speech-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-openapi.yml
- filename: respeecher-openapi.yml
  format: yaml
  label: Respeecher Text-to-Speech API
  slug: respeecher-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-openapi.yml
- filename: respeecher-openapi.yml
  format: yaml
  label: Respeecher Calibration API
  slug: respeecher-calibration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-openapi.yml
- filename: respeecher-openapi.yml
  format: yaml
  label: Respeecher Recordings API
  slug: respeecher-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-openapi.yml
- filename: respeecher-openapi.yml
  format: yaml
  label: Respeecher Projects and Folders API
  slug: respeecher-projects-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-openapi.yml
- filename: respeecher-openapi.yml
  format: yaml
  label: Respeecher Credits API
  slug: respeecher-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-openapi.yml
- filename: respeecher-asyncapi.yml
  format: yaml
  label: Respeecher Space Real-Time TTS API
  slug: respeecher-space-realtime-tts-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/asyncapi/respeecher-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:gr@respeecher.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: respeecher.com
  spf: true
hosts:
- cert_expires: Sep 10 14:00:13 2026 GMT
  host: www.respeecher.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 07:55:52 2026 GMT
  host: docs.respeecher.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 03:30:01 2026 GMT
  host: gateway.respeecher.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Respeecher Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Respeecher, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Respeecher
provider_slug: respeecher
slug: respeecher-domain-security
source_filename: respeecher-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.respeecher.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 14:00:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.respeecher.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 07:55:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gateway.respeecher.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 03:30:01 2026 GMT\n  hsts: null\ndomains:\n- domain: respeecher.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:gr@respeecher.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/security/respeecher-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Voice AI
- Voice Cloning
- Speech to Speech
- Text to Speech
- Voice Conversion
- Real Time
- Media and Entertainment
---
