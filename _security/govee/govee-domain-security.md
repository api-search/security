---
api_specs:
- filename: govee-openapi.yml
  format: yaml
  label: Govee Devices API
  slug: govee-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govee/refs/heads/main/openapi/govee-openapi.yml
- filename: govee-openapi.yml
  format: yaml
  label: Govee Device State API
  slug: govee-device-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govee/refs/heads/main/openapi/govee-openapi.yml
- filename: govee-openapi.yml
  format: yaml
  label: Govee Device Control API
  slug: govee-device-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govee/refs/heads/main/openapi/govee-openapi.yml
- filename: govee-openapi.yml
  format: yaml
  label: Govee Dynamic Scenes API
  slug: govee-dynamic-scenes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govee/refs/heads/main/openapi/govee-openapi.yml
- filename: govee-openapi.yml
  format: yaml
  label: Govee DIY Scenes API
  slug: govee-diy-scenes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govee/refs/heads/main/openapi/govee-openapi.yml
- filename: govee-openapi.yml
  format: yaml
  label: Govee Segment Color and Brightness API
  slug: govee-segment-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govee/refs/heads/main/openapi/govee-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: govee.com
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: www.govee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 09:01:51 2026 GMT
  host: developer.govee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: openapi.api.govee.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Govee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Govee, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Govee
provider_slug: govee
slug: govee-domain-security
source_filename: govee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.govee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.govee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 09:01:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: openapi.api.govee.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: govee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/govee/refs/heads/main/security/govee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Smart Home
- Smart Lighting
- IoT
- LED
- Home Automation
- Device Control
---
