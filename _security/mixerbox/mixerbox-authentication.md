---
api_key_in: []
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
auth_types:
- none
- service_http
description: ''
kind: authentication
layout: security
method: searched
name: Mixerbox Authentication
name_suffix: Authentication
oauth_flows: []
overview: MixerBox secures its APIs with none and service_http across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MixerBox
provider_slug: mixerbox
scheme_count: 0
schemes: []
slug: mixerbox-authentication
source_filename: mixerbox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: well-known/mixerbox-*-ai-plugin.json (OpenAI plugin manifests)\nsummary:\n  types:\n  - none\n  - service_http\n  detail: 'MixerBox exposes each product as a ChatGPT plugin / GPT Action. Authentication\n    is declared in each ai-plugin.json: ''service_http'' (a service-level bearer token\n    the ChatGPT runtime injects on the plugin''s behalf; end users do not supply a\n    key) or ''none'' (open GET/POST). No OpenAPI securitySchemes are declared in the\n    specs. MixerBox Calendar additionally exposes Authorize/Logout operations to link\n    a user''s Google Calendar.'\nplugins:\n- plugin: calendar\n  auth_type: service_http\n  api: openapi/mixerbox-calendar-openapi-original.json\n- plugin: chatpdf\n  auth_type: service_http\n  api: openapi/mixerbox-chatpdf-openapi-original.json\n- plugin: diagrams\n  auth_type: service_http\n  api: openapi/mixerbox-diagrams-openapi-original.json\n- plugin: imagegen\n  auth_type: service_http\n\
  \  api: openapi/mixerbox-imagegen-openapi-original.json\n- plugin: oneplayer\n  auth_type: none\n  api: openapi/mixerbox-oneplayer-openapi-original.json\n- plugin: photomagic\n  auth_type: service_http\n  api: openapi/mixerbox-photomagic-openapi-original.json\n- plugin: podcasts\n  auth_type: none\n  api: openapi/mixerbox-podcasts-openapi-original.json\n- plugin: promptpro\n  auth_type: service_http\n  api: openapi/mixerbox-promptpro-openapi-original.json\n- plugin: qr\n  auth_type: service_http\n  api: openapi/mixerbox-qr-openapi-original.json\n- plugin: scholar\n  auth_type: service_http\n  api: openapi/mixerbox-scholar-openapi-original.json\n- plugin: translate\n  auth_type: none\n  api: openapi/mixerbox-translate-openapi-original.json\n- plugin: weather\n  auth_type: none\n  api: openapi/mixerbox-weather-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/authentication/mixerbox-authentication.yml
summary_line: none/service_http · 0 schemes
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
