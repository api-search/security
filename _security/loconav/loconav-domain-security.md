---
api_specs:
- filename: loconav-alert-subscriptions-api-openapi.yml
  format: yaml
  label: LocoNav Alert Subscriptions API
  slug: loconav-alert-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-alert-subscriptions-api-openapi.yml
- filename: loconav-alerts-api-openapi.yml
  format: yaml
  label: LocoNav Alerts API
  slug: loconav-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-alerts-api-openapi.yml
- filename: loconav-alerts-subscriptions-api-openapi.yml
  format: yaml
  label: LocoNav Alerts Subscriptions API
  slug: loconav-alerts-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-alerts-subscriptions-api-openapi.yml
- filename: loconav-drivers-api-openapi.yml
  format: yaml
  label: LocoNav Drivers API
  slug: loconav-drivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-drivers-api-openapi.yml
- filename: loconav-mobilization-api-openapi.yml
  format: yaml
  label: LocoNav Mobilization API
  slug: loconav-mobilization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-mobilization-api-openapi.yml
- filename: loconav-polygon-geofence-api-openapi.yml
  format: yaml
  label: LocoNav Polygon (Geofence) API
  slug: loconav-polygon-geofence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-polygon-geofence-api-openapi.yml
- filename: loconav-trips-api-openapi.yml
  format: yaml
  label: LocoNav Trips API
  slug: loconav-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-trips-api-openapi.yml
- filename: loconav-users-api-openapi.yml
  format: yaml
  label: LocoNav Users API
  slug: loconav-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-users-api-openapi.yml
- filename: loconav-vehicles-api-openapi.yml
  format: yaml
  label: LocoNav Vehicles API
  slug: loconav-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-vehicles-api-openapi.yml
- filename: loconav-vehicles-telematics-api-openapi.yml
  format: yaml
  label: LocoNav Vehicles / Telematics API
  slug: loconav-vehicles-telematics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-vehicles-telematics-api-openapi.yml
- filename: loconav-video-telematics-vt-live-stream-api-openapi.yml
  format: yaml
  label: LocoNav Video Telematics VT / Live Stream API
  slug: loconav-video-telematics-vt-live-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-video-telematics-vt-live-stream-api-openapi.yml
- filename: loconav-video-telematics-vt-videos-api-openapi.yml
  format: yaml
  label: LocoNav Video Telematics VT / Videos API
  slug: loconav-video-telematics-vt-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-video-telematics-vt-videos-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: loconav.com
  spf: true
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: loconav.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 24 18:19:11 2026 GMT
  host: developers.loconav.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: api.a.loconav.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Loconav Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LocoNav, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LocoNav
provider_slug: loconav
slug: loconav-domain-security
source_filename: loconav-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: loconav.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: false\n- host: developers.loconav.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 18:19:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.a.loconav.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: loconav.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/security/loconav-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Fleet Management
- Telematics
- GPS Tracking
- Vehicle Tracking
- Transportation
- Logistics
- IoT
- Video Telematics
- Webhooks
---
