---
api_specs:
- filename: mixerbox-oneplayer-openapi-original.json
  format: json
  label: MixerBox OnePlayer
  slug: mixerbox-oneplayer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-oneplayer-openapi-original.json
- filename: mixerbox-podcasts-openapi-original.json
  format: json
  label: MixerBox Podcasts
  slug: mixerbox-podcasts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-podcasts-openapi-original.json
- filename: mixerbox-weather-openapi-original.json
  format: json
  label: MixerBox Weather
  slug: mixerbox-weather
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-weather-openapi-original.json
- filename: mixerbox-calendar-openapi-original.json
  format: json
  label: MixerBox Calendar
  slug: mixerbox-calendar
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-calendar-openapi-original.json
- filename: mixerbox-translate-openapi-original.json
  format: json
  label: MixerBox Translate
  slug: mixerbox-translate
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-translate-openapi-original.json
- filename: mixerbox-imagegen-openapi-original.json
  format: json
  label: MixerBox ImageGen
  slug: mixerbox-imagegen
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-imagegen-openapi-original.json
- filename: mixerbox-photomagic-openapi-original.json
  format: json
  label: MixerBox PhotoMagic
  slug: mixerbox-photomagic
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-photomagic-openapi-original.json
- filename: mixerbox-chatpdf-openapi-original.json
  format: json
  label: MixerBox ChatPDF
  slug: mixerbox-chatpdf
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-chatpdf-openapi-original.json
- filename: mixerbox-scholar-openapi-original.json
  format: json
  label: MixerBox Scholar
  slug: mixerbox-scholar
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-scholar-openapi-original.json
- filename: mixerbox-qr-openapi-original.json
  format: json
  label: MixerBox QR
  slug: mixerbox-qr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-qr-openapi-original.json
- filename: mixerbox-diagrams-openapi-original.json
  format: json
  label: MixerBox Diagrams
  slug: mixerbox-diagrams
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-diagrams-openapi-original.json
- filename: mixerbox-promptpro-openapi-original.json
  format: json
  label: MixerBox Prompt Pro
  slug: mixerbox-prompt-pro
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-promptpro-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mixerbox.com
  spf: true
hosts:
- cert_expires: Jan 25 23:59:59 2027 GMT
  host: mixerbox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: calendar.mixerbox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: chatpdf.mixerbox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mixerbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MixerBox, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MixerBox
provider_slug: mixerbox
slug: mixerbox-domain-security
source_filename: mixerbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mixerbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 23:59:59 2027 GMT\n  hsts: false\n- host: calendar.mixerbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: false\n- host: chatpdf.mixerbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: mixerbox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/security/mixerbox-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Artificial Intelligence
- ChatGPT Plugins
- GPT Actions
- Music
- Podcasts
- Weather
- Translation
- Productivity
---
