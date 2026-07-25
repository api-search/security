---
api_specs:
- filename: mixerbox-gpt-api-openapi.yml
  format: yaml
  label: MixerBox Gpt API
  slug: mixerbox-gpt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-gpt-api-openapi.yml
- filename: mixerbox-gpt-plugins-api-openapi.yml
  format: yaml
  label: MixerBox Gpt Plugins API
  slug: mixerbox-gpt-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-gpt-plugins-api-openapi.yml
- filename: mixerbox-services-funcs-getweatherinfo-mobile-0-api-openapi.yml
  format: yaml
  label: MixerBox Services?funcs=GetWeatherInfo&mobile=0 API
  slug: mixerbox-services-funcs-getweatherinfo-mobile-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-services-funcs-getweatherinfo-mobile-0-api-openapi.yml
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
