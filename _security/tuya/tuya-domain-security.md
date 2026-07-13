---
api_specs:
- filename: tuya-device-management-openapi.yml
  format: yaml
  label: Tuya Device Management API
  slug: device-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tuya/refs/heads/main/openapi/tuya-device-management-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tuya.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: tuyaus.com
  spf: false
hosts:
- cert_expires: Sep  1 07:52:36 2026 GMT
  host: developer.tuya.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 07:52:36 2026 GMT
  host: iot.tuya.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 03:32:32 2026 GMT
  host: openapi.tuyaus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tuya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tuya, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tuya
provider_slug: tuya
slug: tuya-domain-security
source_filename: tuya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.tuya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 07:52:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: iot.tuya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 07:52:36 2026 GMT\n  hsts: null\n- host: openapi.tuyaus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 03:32:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tuya.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tuyaus.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tuya/refs/heads/main/security/tuya-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- IoT
- Smart Home
- Devices
- Cloud Platform
- Automation
- Industrial IoT
- Device Management
---
