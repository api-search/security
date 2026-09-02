---
api_specs:
- filename: respeecher-asyncapi.yml
  format: yaml
  label: Respeecher Space Real-Time TTS API
  slug: respeecher-space-realtime-tts-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/asyncapi/respeecher-asyncapi.yml
- filename: respeecher-accents-api-openapi.yml
  format: yaml
  label: Respeecher accents API
  slug: respeecher-accents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-accents-api-openapi.yml
- filename: respeecher-auth-api-openapi.yml
  format: yaml
  label: Respeecher auth API
  slug: respeecher-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-auth-api-openapi.yml
- filename: respeecher-calibration-api-openapi.yml
  format: yaml
  label: Respeecher calibration API
  slug: respeecher-calibration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-calibration-api-openapi.yml
- filename: respeecher-credits-api-openapi.yml
  format: yaml
  label: Respeecher credits API
  slug: respeecher-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-credits-api-openapi.yml
- filename: respeecher-folders-api-openapi.yml
  format: yaml
  label: Respeecher folders API
  slug: respeecher-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-folders-api-openapi.yml
- filename: respeecher-healtz-api-openapi.yml
  format: yaml
  label: Respeecher healtz API
  slug: respeecher-healtz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-healtz-api-openapi.yml
- filename: respeecher-models-api-openapi.yml
  format: yaml
  label: Respeecher models API
  slug: respeecher-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-models-api-openapi.yml
- filename: respeecher-narration-styles-api-openapi.yml
  format: yaml
  label: Respeecher narration-styles API
  slug: respeecher-narration-styles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-narration-styles-api-openapi.yml
- filename: respeecher-notes-api-openapi.yml
  format: yaml
  label: Respeecher notes API
  slug: respeecher-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-notes-api-openapi.yml
- filename: respeecher-orders-api-openapi.yml
  format: yaml
  label: Respeecher orders API
  slug: respeecher-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-orders-api-openapi.yml
- filename: respeecher-projects-api-openapi.yml
  format: yaml
  label: Respeecher projects API
  slug: respeecher-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-projects-api-openapi.yml
- filename: respeecher-recordings-api-openapi.yml
  format: yaml
  label: Respeecher recordings API
  slug: respeecher-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-recordings-api-openapi.yml
- filename: respeecher-stats-api-openapi.yml
  format: yaml
  label: Respeecher stats API
  slug: respeecher-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-stats-api-openapi.yml
- filename: respeecher-storage-api-openapi.yml
  format: yaml
  label: Respeecher storage API
  slug: respeecher-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-storage-api-openapi.yml
- filename: respeecher-tts-api-openapi.yml
  format: yaml
  label: Respeecher tts API
  slug: respeecher-tts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-tts-api-openapi.yml
- filename: respeecher-voices-api-openapi.yml
  format: yaml
  label: Respeecher voices API
  slug: respeecher-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respeecher/refs/heads/main/openapi/respeecher-voices-api-openapi.yml
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
- Text-to-Speech
- Voice Conversion
- Real-Time
- Media and Entertainment
---
