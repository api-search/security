---
api_specs:
- filename: google-display-video-360-api-openapi.yml
  format: yaml
  label: Google Display & Video 360 API
  slug: google-display-video-360-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-display-video-360/refs/heads/main/openapi/google-display-video-360-api-openapi.yml
- filename: google-display-video-360-advertisers-api-openapi.yml
  format: yaml
  label: Google Display & Video 360 Advertisers API
  slug: google-display-video-360-advertisers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-display-video-360/refs/heads/main/openapi/google-display-video-360-advertisers-api-openapi.yml
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
- cert_expires: Oct 12 18:05:55 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 18:07:34 2026 GMT
  host: displayvideo.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Display Video 360 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Display & Video 360, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Display & Video 360
provider_slug: google-display-video-360
slug: google-display-video-360-domain-security
source_filename: google-display-video-360-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 18:05:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: displayvideo.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 18:07:34 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-display-video-360/refs/heads/main/security/google-display-video-360-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Campaign Management
- Display Ads
- DV360
- Programmatic Advertising
- Targeting
- Video Ads
- Advertising
- AdTech
- Demand Side Platform
- Media Buying
- Audiences
- Google Marketing Platform
---
