---
api_specs:
- filename: reference
  format: yaml
  label: Twitch API
  slug: twitch-api
  spec_type: OpenAPI
  url: https://dev.twitch.tv/docs/api/reference
- filename: twitch-eventsub-asyncapi.yml
  format: yaml
  label: Twitch EventSub
  slug: twitch-eventsub
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitch/refs/heads/main/asyncapi/twitch-eventsub-asyncapi.yml
- filename: twitch-extensions-openapi.yml
  format: yaml
  label: Twitch Extensions API
  slug: twitch-extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitch/refs/heads/main/openapi/twitch-extensions-openapi.yml
- filename: twitch-drops-openapi.yml
  format: yaml
  label: Twitch Drops API
  slug: twitch-drops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitch/refs/heads/main/openapi/twitch-drops-openapi.yml
- filename: twitch-video-broadcast-openapi.yml
  format: yaml
  label: Twitch Video Broadcast API
  slug: twitch-video-broadcast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitch/refs/heads/main/openapi/twitch-video-broadcast-openapi.yml
- filename: twitch-insights-analytics-openapi.yml
  format: yaml
  label: Twitch Insights and Analytics API
  slug: twitch-insights-and-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitch/refs/heads/main/openapi/twitch-insights-analytics-openapi.yml
- filename: twitch-igdb-openapi.yml
  format: yaml
  label: IGDB API
  slug: igdb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitch/refs/heads/main/openapi/twitch-igdb-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: twitch.tv
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: dev.twitch.tv
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: api.twitch.tv
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: irc-ws.chat.twitch.tv
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Twitch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Twitch, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Twitch
provider_slug: twitch
slug: twitch-domain-security
source_filename: twitch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dev.twitch.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: false\n- host: api.twitch.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: null\n- host: irc-ws.chat.twitch.tv\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: twitch.tv\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twitch/refs/heads/main/security/twitch-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Entertainment
- Gaming
- Live Video
- Streaming
- Video
---
