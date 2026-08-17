---
api_specs:
- filename: rockbot-audio-messaging-api-openapi.yml
  format: yaml
  label: Rockbot Audio Messaging API
  slug: rockbot-audio-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-audio-messaging-api-openapi.yml
- filename: rockbot-auth-api-openapi.yml
  format: yaml
  label: Rockbot Auth API
  slug: rockbot-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-auth-api-openapi.yml
- filename: rockbot-data-api-openapi.yml
  format: yaml
  label: Rockbot Data API
  slug: rockbot-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-data-api-openapi.yml
- filename: rockbot-devices-api-openapi.yml
  format: yaml
  label: Rockbot Devices API
  slug: rockbot-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-devices-api-openapi.yml
- filename: rockbot-music-api-openapi.yml
  format: yaml
  label: Rockbot Music API
  slug: rockbot-music-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-music-api-openapi.yml
- filename: rockbot-signage-api-openapi.yml
  format: yaml
  label: Rockbot Signage API
  slug: rockbot-signage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-signage-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 128 issuewild "comodoca.com"
  - 0 issue "pki.goog"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rockbot.com
  spf: true
hosts:
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: rockbot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: developer.rockbot.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: api.rockbot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rockbot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rockbot, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rockbot
provider_slug: rockbot
slug: rockbot-domain-security
source_filename: rockbot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rockbot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.rockbot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: false\n- host: api.rockbot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rockbot.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 128 issuewild \"comodoca.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/security/rockbot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Music
- Digital Signage
- Audio Messaging
- Retail Media
- In-Location Media
- Media
- Entertainment
---
