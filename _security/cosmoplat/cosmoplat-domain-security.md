---
api_specs:
- filename: cosmoplat-iot-platform-openapi.yml
  format: yaml
  label: COSMOPlat IoT Platform OpenAPI
  slug: cosmoplat-iot-platform-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmoplat/refs/heads/main/openapi/cosmoplat-iot-platform-openapi.yml
- filename: cosmoplat-iot-telemetry-asyncapi.yml
  format: yaml
  label: COSMOPlat IoT Telemetry (MQTT)
  slug: cosmoplat-iot-telemetry-mqtt
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmoplat/refs/heads/main/asyncapi/cosmoplat-iot-telemetry-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cosmoplat.com
  spf: true
hosts:
- cert_expires: Mar  3 09:39:30 2027 GMT
  host: www.cosmoplat.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  3 09:39:30 2027 GMT
  host: iot-mqtt.cosmoplat.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cosmoplat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cosmoplat, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cosmoplat
provider_slug: cosmoplat
slug: cosmoplat-domain-security
source_filename: cosmoplat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cosmoplat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  3 09:39:30 2027 GMT\n  hsts: false\n- host: iot-mqtt.cosmoplat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  3 09:39:30 2027 GMT\n  hsts: null\ndomains:\n- domain: cosmoplat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cosmoplat/refs/heads/main/security/cosmoplat-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Industrial Internet
- Industrial IoT
- Internet of Things
- Manufacturing
- Smart Factory
- Device Management
- Digital Transformation
- MQTT
- Telemetry
- China
---
