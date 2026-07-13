---
api_specs:
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Activities API
  slug: youtube-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Channels API
  slug: youtube-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Comments API
  slug: youtube-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Comment Threads API
  slug: youtube-comment-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Playlists API
  slug: youtube-playlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Playlist Items API
  slug: youtube-playlist-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Search API
  slug: youtube-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Subscriptions API
  slug: youtube-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Videos API
  slug: youtube-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Captions API
  slug: youtube-captions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Video Categories API
  slug: youtube-video-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube I18n Languages API
  slug: youtube-i18n-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube I18n Regions API
  slug: youtube-i18n-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-analytics-openapi.yml
  format: yaml
  label: YouTube Analytics API
  slug: youtube-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-analytics-openapi.yml
- filename: youtube-reporting-openapi.yml
  format: yaml
  label: YouTube Reporting API
  slug: youtube-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-reporting-openapi.yml
- filename: youtube-live-streaming-openapi.yml
  format: yaml
  label: YouTube Live Streaming API
  slug: youtube-live-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-live-streaming-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: www.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: youtubeanalytics.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Youtube Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Youtube, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Youtube
provider_slug: youtube
slug: youtube-domain-security
source_filename: youtube-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\n- host: youtubeanalytics.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/security/youtube-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
---
