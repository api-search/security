---
api_specs:
- filename: bear-robotics-carti-api-openapi.yml
  format: yaml
  label: Bear Robotics Carti API
  slug: bear-robotics-carti-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-carti-api-openapi.yml
- filename: bear-robotics-fleet-management-api-openapi.yml
  format: yaml
  label: Bear Robotics Fleet Management API
  slug: bear-robotics-fleet-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-fleet-management-api-openapi.yml
- filename: bear-robotics-localization-navigation-api-openapi.yml
  format: yaml
  label: Bear Robotics Localization & Navigation API
  slug: bear-robotics-localization-navigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-localization-navigation-api-openapi.yml
- filename: bear-robotics-locations-maps-api-openapi.yml
  format: yaml
  label: Bear Robotics Locations & Maps API
  slug: bear-robotics-locations-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-locations-maps-api-openapi.yml
- filename: bear-robotics-mission-api-openapi.yml
  format: yaml
  label: Bear Robotics Mission API
  slug: bear-robotics-mission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-mission-api-openapi.yml
- filename: bear-robotics-robot-status-api-openapi.yml
  format: yaml
  label: Bear Robotics Robot Status API
  slug: bear-robotics-robot-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-robot-status-api-openapi.yml
- filename: bear-robotics-robot-system-api-openapi.yml
  format: yaml
  label: Bear Robotics Robot System API
  slug: bear-robotics-robot-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-robot-system-api-openapi.yml
- filename: bear-robotics-servi-api-openapi.yml
  format: yaml
  label: Bear Robotics Servi API
  slug: bear-robotics-servi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-servi-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forgeglobal.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bearrobotics.ai
  spf: true
hosts:
- cert_expires: Oct 19 20:15:48 2026 GMT
  host: forgeglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 17:06:45 2026 GMT
  host: api.bearrobotics.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bear Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bear Robotics, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bear Robotics
provider_slug: bear-robotics
slug: bear-robotics-domain-security
source_filename: bear-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forgeglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 20:15:48 2026 GMT\n  hsts: null\n- host: api.bearrobotics.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 17:06:45 2026 GMT\n  hsts: null\ndomains:\n- domain: forgeglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: bearrobotics.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/security/bear-robotics-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Robotics
- Autonomous Mobile Robots
- Fleet Management
- Hospitality
- Food Service
- Logistics
- gRPC
- Protobuf
- Webhooks
- Internet of Things
- Company
---
