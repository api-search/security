---
api_specs:
- filename: hypertrack-openapi.yaml
  format: yaml
  label: HyperTrack API
  slug: hypertrack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hypertrack/refs/heads/main/openapi/hypertrack-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hypertrack.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: hypertrack.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: v3.api.hypertrack.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hypertrack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HyperTrack, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HyperTrack
provider_slug: hypertrack
slug: hypertrack-domain-security
source_filename: hypertrack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hypertrack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: false\n- host: v3.api.hypertrack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hypertrack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hypertrack/refs/heads/main/security/hypertrack-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Location
- Geolocation
- Tracking
- Logistics
- Last Mile Delivery
- Field Service
- Workforce
- Time and Attendance
- Mobile SDK
- Geofencing
- Routing
---
