---
api_specs:
- filename: thingsboard-devices-openapi.yml
  format: yaml
  label: ThingsBoard Devices API
  slug: thingsboard-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-devices-openapi.yml
- filename: thingsboard-assets-openapi.yml
  format: yaml
  label: ThingsBoard Assets API
  slug: thingsboard-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-assets-openapi.yml
- filename: thingsboard-telemetry-openapi.yml
  format: yaml
  label: ThingsBoard Telemetry API
  slug: thingsboard-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-telemetry-openapi.yml
- filename: thingsboard-alarms-openapi.yml
  format: yaml
  label: ThingsBoard Alarms API
  slug: thingsboard-alarms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-alarms-openapi.yml
- filename: thingsboard-rule-engine-openapi.yml
  format: yaml
  label: ThingsBoard Rule Engine API
  slug: thingsboard-rule-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-rule-engine-openapi.yml
- filename: thingsboard-rpc-openapi.yml
  format: yaml
  label: ThingsBoard RPC API
  slug: thingsboard-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-rpc-openapi.yml
- filename: thingsboard-dashboards-openapi.yml
  format: yaml
  label: ThingsBoard Dashboards API
  slug: thingsboard-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-dashboards-openapi.yml
- filename: thingsboard-auth-openapi.yml
  format: yaml
  label: ThingsBoard Authentication API
  slug: thingsboard-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-auth-openapi.yml
- filename: thingsboard-tenants-openapi.yml
  format: yaml
  label: ThingsBoard Tenants and Customers API
  slug: thingsboard-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-tenants-openapi.yml
- filename: thingsboard-admin-openapi.yml
  format: yaml
  label: ThingsBoard Admin API
  slug: thingsboard-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-admin-openapi.yml
- filename: thingsboard-notifications-openapi.yml
  format: yaml
  label: ThingsBoard Notifications API
  slug: thingsboard-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-notifications-openapi.yml
- filename: thingsboard-edge-openapi.yml
  format: yaml
  label: ThingsBoard Edge API
  slug: thingsboard-edge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-edge-openapi.yml
- filename: thingsboard-mobile-openapi.yml
  format: yaml
  label: ThingsBoard Mobile App API
  slug: thingsboard-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-mobile-openapi.yml
- filename: thingsboard-lwm2m-openapi.yml
  format: yaml
  label: ThingsBoard LwM2M API
  slug: thingsboard-lwm2m-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-lwm2m-openapi.yml
- filename: thingsboard-ai-openapi.yml
  format: yaml
  label: ThingsBoard AI API
  slug: thingsboard-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thingsboard.io
  spf: true
hosts:
- cert_expires: Oct  9 14:17:01 2026 GMT
  host: thingsboard.io
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 11:13:59 2026 GMT
  host: demo.thingsboard.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thingsboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ThingsBoard, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ThingsBoard
provider_slug: thingsboard
slug: thingsboard-domain-security
source_filename: thingsboard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thingsboard.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 14:17:01 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: demo.thingsboard.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 11:13:59 2026 GMT\n  hsts: false\ndomains:\n- domain: thingsboard.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/security/thingsboard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- IoT
- Internet of Things
- Device Management
- Telemetry
- Open Source
- Apache 2.0
- MQTT
- LwM2M
- CoAP
- Rule Engine
- Dashboards
- Edge
- Multi-tenant
- Java
- Spring
---
