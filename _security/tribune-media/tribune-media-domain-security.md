---
api_specs:
- filename: tribune-media-celebrities-api-openapi.yml
  format: yaml
  label: Tribune Media Celebrities API
  slug: tribune-media-celebrities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/openapi/tribune-media-celebrities-api-openapi.yml
- filename: tribune-media-lineups-api-openapi.yml
  format: yaml
  label: Tribune Media Lineups API
  slug: tribune-media-lineups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/openapi/tribune-media-lineups-api-openapi.yml
- filename: tribune-media-movies-api-openapi.yml
  format: yaml
  label: Tribune Media Movies API
  slug: tribune-media-movies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/openapi/tribune-media-movies-api-openapi.yml
- filename: tribune-media-online-video-api-openapi.yml
  format: yaml
  label: Tribune Media Online Video API
  slug: tribune-media-online-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/openapi/tribune-media-online-video-api-openapi.yml
- filename: tribune-media-programs-api-openapi.yml
  format: yaml
  label: Tribune Media Programs API
  slug: tribune-media-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/openapi/tribune-media-programs-api-openapi.yml
- filename: tribune-media-series-api-openapi.yml
  format: yaml
  label: Tribune Media Series API
  slug: tribune-media-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/openapi/tribune-media-series-api-openapi.yml
- filename: tribune-media-social-api-openapi.yml
  format: yaml
  label: Tribune Media Social API
  slug: tribune-media-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/openapi/tribune-media-social-api-openapi.yml
- filename: tribune-media-sports-api-openapi.yml
  format: yaml
  label: Tribune Media Sports API
  slug: tribune-media-sports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/openapi/tribune-media-sports-api-openapi.yml
- filename: tribune-media-stations-api-openapi.yml
  format: yaml
  label: Tribune Media Stations API
  slug: tribune-media-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/openapi/tribune-media-stations-api-openapi.yml
- filename: tribune-media-theatres-api-openapi.yml
  format: yaml
  label: Tribune Media Theatres API
  slug: tribune-media-theatres-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/openapi/tribune-media-theatres-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tribunemedia.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: tmsapi.com
  spf: false
hosts:
- cert_expires: Sep  3 05:23:37 2026 GMT
  host: www.tribunemedia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 13:11:20 2026 GMT
  host: developer.tmsapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 13:11:20 2026 GMT
  host: data.tmsapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tribune Media Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tribune Media, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tribune Media
provider_slug: tribune-media
slug: tribune-media-domain-security
source_filename: tribune-media-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tribunemedia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 05:23:37 2026 GMT\n  hsts: false\n- host: developer.tmsapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 13:11:20 2026 GMT\n  hsts: false\n- host: data.tmsapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 13:11:20 2026 GMT\n  hsts: null\ndomains:\n- domain: tribunemedia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tmsapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/security/tribune-media-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Media
- Entertainment
- Broadcasting
- Television
- Movies
- Sports
- Celebrity
- Fortune 1000
---
