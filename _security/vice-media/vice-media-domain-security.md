---
api_specs:
- filename: vice-media-wp-rest-openapi.yml
  format: yaml
  label: VICE WordPress REST API
  slug: vice-media-wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vice-media/refs/heads/main/openapi/_ae-authored/vice-media-wp-rest-openapi.yml
- filename: vice-media-video-wp-rest-openapi.yml
  format: yaml
  label: VICE Video WordPress REST API
  slug: vice-media-video-wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vice-media/refs/heads/main/openapi/_ae-authored/vice-media-video-wp-rest-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vice.com
  spf: true
hosts:
- cert_expires: Oct  8 13:56:49 2026 GMT
  host: www.vice.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 05:55:57 2026 GMT
  host: video.vice.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: api.vice.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Vice Media Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vice Media, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vice Media
provider_slug: vice-media
slug: vice-media-domain-security
source_filename: vice-media-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 13:56:49 2026 GMT\n  hsts: false\n- host: video.vice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 05:55:57 2026 GMT\n  hsts: false\n- host: api.vice.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vice.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vice-media/refs/heads/main/security/vice-media-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Media
- Publishing
- News
- Digital Media
- Content
- Video
- Entertainment
- WordPress
- Syndication
- oEmbed
- Brooklyn
---
