---
api_specs:
- filename: rhombus-systems-openapi.json
  format: json
  label: Rhombus Public REST API
  slug: rhombus-systems-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhombus-systems/refs/heads/main/openapi/rhombus-systems-openapi.json
- filename: rhombus-systems-console-websocket-asyncapi.json
  format: json
  label: Rhombus Console WebSocket API
  slug: rhombus-systems-console-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhombus-systems/refs/heads/main/asyncapi/rhombus-systems-console-websocket-asyncapi.json
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rhombus.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: rhombus.community
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: www.rhombus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 19:42:18 2026 GMT
  host: api-docs.rhombus.community
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: api2.rhombussystems.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Rhombus Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rhombus Systems, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rhombus Systems
provider_slug: rhombus-systems
slug: rhombus-systems-domain-security
source_filename: rhombus-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rhombus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.rhombus.community\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 19:42:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api2.rhombussystems.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: rhombus.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: rhombus.community\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rhombus-systems/refs/heads/main/security/rhombus-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Physical Security
- Video Surveillance
- Access Control
- IoT Sensors
- Cloud Video Management
- Alarm Monitoring
- Computer Vision
- Building Management
- Security Cameras
- Company
---
