---
api_specs:
- filename: franklin-whole-home-authentication-api-openapi.yml
  format: yaml
  label: Franklin Whole Home Authentication API
  slug: franklin-whole-home-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/franklin-whole-home/refs/heads/main/openapi/franklin-whole-home-authentication-api-openapi.yml
- filename: franklin-whole-home-device-data-api-openapi.yml
  format: yaml
  label: Franklin Whole Home Device Data API
  slug: franklin-whole-home-device-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/franklin-whole-home/refs/heads/main/openapi/franklin-whole-home-device-data-api-openapi.yml
- filename: franklin-whole-home-devices-api-openapi.yml
  format: yaml
  label: Franklin Whole Home Devices API
  slug: franklin-whole-home-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/franklin-whole-home/refs/heads/main/openapi/franklin-whole-home-devices-api-openapi.yml
- filename: franklin-whole-home-grid-events-api-openapi.yml
  format: yaml
  label: Franklin Whole Home Grid Events API
  slug: franklin-whole-home-grid-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/franklin-whole-home/refs/heads/main/openapi/franklin-whole-home-grid-events-api-openapi.yml
- filename: franklin-whole-home-groups-api-openapi.yml
  format: yaml
  label: Franklin Whole Home Groups API
  slug: franklin-whole-home-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/franklin-whole-home/refs/heads/main/openapi/franklin-whole-home-groups-api-openapi.yml
- filename: franklin-whole-home-modification-records-api-openapi.yml
  format: yaml
  label: Franklin Whole Home Modification Records API
  slug: franklin-whole-home-modification-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/franklin-whole-home/refs/heads/main/openapi/franklin-whole-home-modification-records-api-openapi.yml
- filename: franklin-whole-home-sites-api-openapi.yml
  format: yaml
  label: Franklin Whole Home Sites API
  slug: franklin-whole-home-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/franklin-whole-home/refs/heads/main/openapi/franklin-whole-home-sites-api-openapi.yml
- filename: franklin-whole-home-sunrun-api-openapi.yml
  format: yaml
  label: Franklin Whole Home Sunrun API
  slug: franklin-whole-home-sunrun-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/franklin-whole-home/refs/heads/main/openapi/franklin-whole-home-sunrun-api-openapi.yml
- filename: franklin-whole-home-sunrun-sites-api-openapi.yml
  format: yaml
  label: Franklin Whole Home Sunrun Sites API
  slug: franklin-whole-home-sunrun-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/franklin-whole-home/refs/heads/main/openapi/franklin-whole-home-sunrun-sites-api-openapi.yml
- filename: franklin-whole-home-sunrun-system-setup-api-openapi.yml
  format: yaml
  label: Franklin Whole Home Sunrun System Setup API
  slug: franklin-whole-home-sunrun-system-setup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/franklin-whole-home/refs/heads/main/openapi/franklin-whole-home-sunrun-system-setup-api-openapi.yml
- filename: franklin-whole-home-system-settings-api-openapi.yml
  format: yaml
  label: Franklin Whole Home System Settings API
  slug: franklin-whole-home-system-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/franklin-whole-home/refs/heads/main/openapi/franklin-whole-home-system-settings-api-openapi.yml
- filename: franklin-whole-home-warnings-and-events-api-openapi.yml
  format: yaml
  label: Franklin Whole Home Warnings and Events API
  slug: franklin-whole-home-warnings-and-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/franklin-whole-home/refs/heads/main/openapi/franklin-whole-home-warnings-and-events-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: franklinwh.com
  spf: true
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: www.franklinwh.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 09:03:41 2026 GMT
  host: api.franklinwh.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 09:03:41 2026 GMT
  host: test-api.franklinwh.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Franklin Whole Home Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Franklin Whole Home, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Franklin Whole Home
provider_slug: franklin-whole-home
slug: franklin-whole-home-domain-security
source_filename: franklin-whole-home-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.franklinwh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.franklinwh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 09:03:41 2026 GMT\n  hsts: false\n- host: test-api.franklinwh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 09:03:41 2026 GMT\n  hsts: null\ndomains:\n- domain: franklinwh.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/franklin-whole-home/refs/heads/main/security/franklin-whole-home-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Energy Storage
- Home Energy Management
- Solar
- Batteries
- Internet of Things
- Smart Home
- Electric Vehicles
- Cleantech
- Device Telemetry
---
