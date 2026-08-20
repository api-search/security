---
api_specs:
- filename: weavix-channels-messaging-api-openapi.yml
  format: yaml
  label: Weavix Channels & Messaging API
  slug: weavix-channels-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavix/refs/heads/main/openapi/weavix-channels-messaging-api-openapi.yml
- filename: weavix-crafts-api-openapi.yml
  format: yaml
  label: Weavix Crafts API
  slug: weavix-crafts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavix/refs/heads/main/openapi/weavix-crafts-api-openapi.yml
- filename: weavix-forms-api-openapi.yml
  format: yaml
  label: Weavix Forms API
  slug: weavix-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavix/refs/heads/main/openapi/weavix-forms-api-openapi.yml
- filename: weavix-geofences-api-openapi.yml
  format: yaml
  label: Weavix Geofences API
  slug: weavix-geofences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavix/refs/heads/main/openapi/weavix-geofences-api-openapi.yml
- filename: weavix-mass-alerts-api-openapi.yml
  format: yaml
  label: Weavix Mass Alerts API
  slug: weavix-mass-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavix/refs/heads/main/openapi/weavix-mass-alerts-api-openapi.yml
- filename: weavix-permission-groups-api-openapi.yml
  format: yaml
  label: Weavix Permission Groups API
  slug: weavix-permission-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavix/refs/heads/main/openapi/weavix-permission-groups-api-openapi.yml
- filename: weavix-sites-api-openapi.yml
  format: yaml
  label: Weavix Sites API
  slug: weavix-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavix/refs/heads/main/openapi/weavix-sites-api-openapi.yml
- filename: weavix-user-management-api-openapi.yml
  format: yaml
  label: Weavix User Management API
  slug: weavix-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavix/refs/heads/main/openapi/weavix-user-management-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: weavix.com
  spf: true
hosts:
- cert_expires: Sep 29 09:42:50 2026 GMT
  host: weavix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:44:15 2026 GMT
  host: help.weavix.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 14:17:27 2026 GMT
  host: api.weavix.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weavix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weavix, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Weavix
provider_slug: weavix
slug: weavix-domain-security
source_filename: weavix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: weavix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 09:42:50 2026 GMT\n  hsts: false\n- host: help.weavix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:44:15 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: api.weavix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 14:17:27 2026 GMT\n  hsts: null\ndomains:\n- domain: weavix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weavix/refs/heads/main/security/weavix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Communications
- Frontline Workers
- Workforce Management
- Messaging
- Push To Talk
- Industrial
- Internet of Things
- Location Tracking
- Alerts
- Company
---
