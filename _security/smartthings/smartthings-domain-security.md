---
api_specs:
- filename: smartthings-apps-api-openapi.yml
  format: yaml
  label: Samsung SmartThings Apps API
  slug: smartthings-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-apps-api-openapi.yml
- filename: smartthings-capabilities-api-openapi.yml
  format: yaml
  label: Samsung SmartThings Capabilities API
  slug: smartthings-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-capabilities-api-openapi.yml
- filename: smartthings-device-commands-status-api-openapi.yml
  format: yaml
  label: Samsung SmartThings Device Commands & Status API
  slug: smartthings-device-commands-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-device-commands-status-api-openapi.yml
- filename: smartthings-devices-api-openapi.yml
  format: yaml
  label: Samsung SmartThings Devices API
  slug: smartthings-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-devices-api-openapi.yml
- filename: smartthings-history-api-openapi.yml
  format: yaml
  label: Samsung SmartThings History API
  slug: smartthings-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-history-api-openapi.yml
- filename: smartthings-installed-apps-api-openapi.yml
  format: yaml
  label: Samsung SmartThings Installed Apps API
  slug: smartthings-installed-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-installed-apps-api-openapi.yml
- filename: smartthings-locations-api-openapi.yml
  format: yaml
  label: Samsung SmartThings Locations API
  slug: smartthings-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-locations-api-openapi.yml
- filename: smartthings-presentations-api-openapi.yml
  format: yaml
  label: Samsung SmartThings Presentations API
  slug: smartthings-presentations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-presentations-api-openapi.yml
- filename: smartthings-rooms-api-openapi.yml
  format: yaml
  label: Samsung SmartThings Rooms API
  slug: smartthings-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-rooms-api-openapi.yml
- filename: smartthings-rules-api-openapi.yml
  format: yaml
  label: Samsung SmartThings Rules API
  slug: smartthings-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-rules-api-openapi.yml
- filename: smartthings-scenes-api-openapi.yml
  format: yaml
  label: Samsung SmartThings Scenes API
  slug: smartthings-scenes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-scenes-api-openapi.yml
- filename: smartthings-schedules-api-openapi.yml
  format: yaml
  label: Samsung SmartThings Schedules API
  slug: smartthings-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-schedules-api-openapi.yml
- filename: smartthings-subscriptions-api-openapi.yml
  format: yaml
  label: Samsung SmartThings Subscriptions API
  slug: smartthings-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-subscriptions-api-openapi.yml
- filename: smartthings-virtual-devices-api-openapi.yml
  format: yaml
  label: Samsung SmartThings Virtual Devices API
  slug: smartthings-virtual-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-virtual-devices-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smartthings.com
  spf: true
hosts:
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: www.smartthings.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: developer.smartthings.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: api.smartthings.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smartthings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Samsung SmartThings, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Samsung SmartThings
provider_slug: smartthings
slug: smartthings-domain-security
source_filename: smartthings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smartthings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.smartthings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.smartthings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: smartthings.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/security/smartthings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Smart Home
- IoT
- Home Automation
- Devices
- Samsung
---
