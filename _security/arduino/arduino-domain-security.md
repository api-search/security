---
api_specs:
- filename: swagger.json
  format: json
  label: Arduino IoT Cloud API
  slug: arduino-iot-cloud-api
  spec_type: OpenAPI
  url: http://api2.arduino.cc/iot/swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arduino.cc
  spf: true
hosts:
- cert_expires: Oct  6 22:32:29 2026 GMT
  host: www.arduino.cc
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 13:58:33 2026 GMT
  host: docs.arduino.cc
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: api2.arduino.cc
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arduino Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arduino, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Arduino
provider_slug: arduino
slug: arduino-domain-security
source_filename: arduino-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arduino.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:32:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.arduino.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 13:58:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api2.arduino.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: arduino.cc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arduino/refs/heads/main/security/arduino-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- IoT
- Electronics
- Open Source
- Devices
- Dashboards
- Time Series
- Cloud
---
