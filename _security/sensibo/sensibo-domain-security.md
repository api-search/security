---
api_specs:
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo Users API
  slug: sensibo-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo Devices API
  slug: sensibo-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo AC States API
  slug: sensibo-ac-states-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo Measurements API
  slug: sensibo-measurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo Historical Data API
  slug: sensibo-historical-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo Climate React API
  slug: sensibo-climate-react-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo Schedules API
  slug: sensibo-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo Timers API
  slug: sensibo-timers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sensibo.com
  spf: true
hosts:
- cert_expires: Aug 27 01:24:02 2026 GMT
  host: sensibo.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 12:03:21 2026 GMT
  host: support.sensibo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: home.sensibo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sensibo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sensibo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sensibo
provider_slug: sensibo
slug: sensibo-domain-security
source_filename: sensibo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sensibo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 01:24:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: support.sensibo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 12:03:21 2026 GMT\n  hsts: false\n- host: home.sensibo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sensibo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/security/sensibo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Smart Home
- IoT
- Air Conditioning
- HVAC
- Air Quality
- Climate Control
- Connected Devices
---
