---
api_specs:
- filename: dolby-optiview-live-openapi.yml
  format: yaml
  label: Dolby OptiView Live
  slug: optiview-live
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby/refs/heads/main/openapi/dolby-optiview-live-openapi.yml
- filename: dolby-millicast-api-openapi.yml
  format: yaml
  label: Dolby OptiView Real-time Streaming (Millicast)
  slug: real-time-millicast
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby/refs/heads/main/openapi/dolby-millicast-api-openapi.yml
- filename: dolby-millicast-director-openapi.yml
  format: yaml
  label: Dolby OptiView Director API (Millicast)
  slug: millicast-director
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby/refs/heads/main/openapi/dolby-millicast-director-openapi.yml
- filename: dolby-millicast-analytics-openapi.yml
  format: yaml
  label: Dolby OptiView Advanced Analytics API (Millicast)
  slug: millicast-analytics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby/refs/heads/main/openapi/dolby-millicast-analytics-openapi.yml
- filename: dolby-optiview-ads-openapi.yml
  format: yaml
  label: Dolby OptiView Ads
  slug: optiview-ads
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby/refs/heads/main/openapi/dolby-optiview-ads-openapi.yml
- filename: dolby-optiview-ad-engine-openapi.yml
  format: yaml
  label: Dolby OptiView Ad Engine
  slug: optiview-ad-engine
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby/refs/heads/main/openapi/dolby-optiview-ad-engine-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dolby.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: theo.live
  spf: true
hosts:
- cert_expires: Nov  1 01:37:11 2026 GMT
  host: optiview.dolby.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 14:56:50 2026 GMT
  host: api.theo.live
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: api.millicast.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Dolby Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dolby, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dolby
provider_slug: dolby
slug: dolby-domain-security
source_filename: dolby-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: optiview.dolby.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 01:37:11 2026 GMT\n  hsts: false\n- host: api.theo.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:56:50 2026 GMT\n  hsts: null\n- host: api.millicast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: dolby.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: theo.live\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dolby/refs/heads/main/security/dolby-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Audio
- Video
- Streaming
- Media
- Real-Time
- WebRTC
- Advertising
- Video Player
- Live Streaming
- Broadcasting
---
