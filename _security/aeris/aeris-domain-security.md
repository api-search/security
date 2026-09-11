---
api_specs:
- filename: aeris-auth-3.0-openapi.yaml
  format: yaml
  label: Aeris IoT Accelerator REST API
  slug: aeris-iot-accelerator-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeris/refs/heads/main/openapi/aeris-auth-3.0-openapi.yaml
- filename: aeris-sms-messaging-api-openapi.yaml
  format: yaml
  label: Aeris IoT Accelerator SMS Messaging API
  slug: aeris-iot-accelerator-sms-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeris/refs/heads/main/openapi/aeris-sms-messaging-api-openapi.yaml
- filename: aeris-watchtower-api-openapi-openapi.yaml
  format: yaml
  label: Aeris IoT Watchtower API
  slug: aeris-iot-watchtower-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeris/refs/heads/main/openapi/aeris-watchtower-api-openapi-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: aeris.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: aeris.net
  spf: false
hosts:
- cert_expires: Mar 27 23:59:59 2027 GMT
  host: www.aeris.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:45:24 2026 GMT
  host: iotdeveloper.aeris.net
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: iot-api.aeris.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Aeris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aeris, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Aeris
provider_slug: aeris
slug: aeris-domain-security
source_filename: aeris-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aeris.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 27 23:59:59 2027 GMT\n  hsts: false\n- host: iotdeveloper.aeris.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:45:24 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: iot-api.aeris.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: aeris.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: aeris.net\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aeris/refs/heads/main/security/aeris-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- IoT
- Cellular Connectivity
- M2M
- eSIM
- SIM Management
- Telecom
- Device Management
- IoT Security
- Connectivity Management Platform
- SMS Messaging
- eUICC
- Fleet Telematics
---
