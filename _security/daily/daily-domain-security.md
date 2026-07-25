---
api_specs:
- filename: daily-batch-rooms-api-openapi.yml
  format: yaml
  label: Daily batch/rooms API
  slug: daily-batch-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-batch-rooms-api-openapi.yml
- filename: daily-dialin-api-openapi.yml
  format: yaml
  label: Daily dialin API
  slug: daily-dialin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-dialin-api-openapi.yml
- filename: daily-domain-api-openapi.yml
  format: yaml
  label: Daily domain API
  slug: daily-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-domain-api-openapi.yml
- filename: daily-domain-dialin-config-api-openapi.yml
  format: yaml
  label: Daily domain-dialin-config API
  slug: daily-domain-dialin-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-domain-dialin-config-api-openapi.yml
- filename: daily-logs-api-openapi.yml
  format: yaml
  label: Daily logs API
  slug: daily-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-logs-api-openapi.yml
- filename: daily-meeting-tokens-api-openapi.yml
  format: yaml
  label: Daily meeting-tokens API
  slug: daily-meeting-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-meeting-tokens-api-openapi.yml
- filename: daily-meetings-api-openapi.yml
  format: yaml
  label: Daily meetings API
  slug: daily-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-meetings-api-openapi.yml
- filename: daily-phone-numbers-api-openapi.yml
  format: yaml
  label: Daily phone-numbers API
  slug: daily-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-phone-numbers-api-openapi.yml
- filename: daily-presence-api-openapi.yml
  format: yaml
  label: Daily presence API
  slug: daily-presence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-presence-api-openapi.yml
- filename: daily-recordings-api-openapi.yml
  format: yaml
  label: Daily recordings API
  slug: daily-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-recordings-api-openapi.yml
- filename: daily-rooms-api-openapi.yml
  format: yaml
  label: Daily rooms API
  slug: daily-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-rooms-api-openapi.yml
- filename: daily-transcript-api-openapi.yml
  format: yaml
  label: Daily transcript API
  slug: daily-transcript-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-transcript-api-openapi.yml
- filename: daily-webhooks-api-openapi.yml
  format: yaml
  label: Daily webhooks API
  slug: daily-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:help@daily.co"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: daily.co
  spf: true
hosts:
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: api.daily.co
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Daily Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Daily, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Daily
provider_slug: daily
slug: daily-domain-security
source_filename: daily-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.daily.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: daily.co\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:help@daily.co\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/security/daily-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Video
- Audio
- WebRTC
- Real-Time Communication
- Video Conferencing
- Live Streaming
- Recording
- Transcription
- Telephony
- SIP
- PSTN
- Company
---
