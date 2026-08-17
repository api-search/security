---
api_specs:
- filename: paedae-applications-api-openapi.yml
  format: yaml
  label: Paedae Applications API
  slug: paedae-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-applications-api-openapi.yml
- filename: paedae-beacon-configurations-api-openapi.yml
  format: yaml
  label: Paedae Beacon Configurations API
  slug: paedae-beacon-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-beacon-configurations-api-openapi.yml
- filename: paedae-beacons-api-openapi.yml
  format: yaml
  label: Paedae Beacons API
  slug: paedae-beacons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-beacons-api-openapi.yml
- filename: paedae-communications-api-openapi.yml
  format: yaml
  label: Paedae Communications API
  slug: paedae-communications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-communications-api-openapi.yml
- filename: paedae-places-api-openapi.yml
  format: yaml
  label: Paedae Places API
  slug: paedae-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-places-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gimbal.com
  spf: true
hosts:
- cert_expires: Nov  9 20:51:49 2026 GMT
  host: www.gimbal.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: manager.gimbal.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: docs.gimbal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paedae Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paedae, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Paedae
provider_slug: paedae
slug: paedae-domain-security
source_filename: paedae-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gimbal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 20:51:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: manager.gimbal.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: null\n- host: docs.gimbal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: gimbal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/security/paedae-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Proximity
- Location
- Beacons
- Geofencing
- Mobile SDK
- Advertising
- Marketing
---
