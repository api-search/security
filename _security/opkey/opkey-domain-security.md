---
api_specs:
- filename: opkey-apk-instrumentation-api-openapi.yml
  format: yaml
  label: Opkey Apk Instrumentation API
  slug: opkey-apk-instrumentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-apk-instrumentation-api-openapi.yml
- filename: opkey-apk-instrumentation-apis-api-openapi.yml
  format: yaml
  label: Opkey Apk Instrumentation Apis API
  slug: opkey-apk-instrumentation-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-apk-instrumentation-apis-api-openapi.yml
- filename: opkey-app-center-api-api-openapi.yml
  format: yaml
  label: Opkey App Center Api API
  slug: opkey-app-center-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-app-center-api-api-openapi.yml
- filename: opkey-app-control-api-openapi.yml
  format: yaml
  label: Opkey App Control API
  slug: opkey-app-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-app-control-api-openapi.yml
- filename: opkey-appium-automation-api-openapi.yml
  format: yaml
  label: Opkey Appium Automation API
  slug: opkey-appium-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-appium-automation-api-openapi.yml
- filename: opkey-authentication-api-openapi.yml
  format: yaml
  label: Opkey Authentication API
  slug: opkey-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-authentication-api-openapi.yml
- filename: opkey-device-booking-session-api-openapi.yml
  format: yaml
  label: Opkey Device Booking & Session API
  slug: opkey-device-booking-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-device-booking-session-api-openapi.yml
- filename: opkey-device-interaction-api-openapi.yml
  format: yaml
  label: Opkey Device Interaction API
  slug: opkey-device-interaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-device-interaction-api-openapi.yml
- filename: opkey-file-management-api-openapi.yml
  format: yaml
  label: Opkey File Management API
  slug: opkey-file-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-file-management-api-openapi.yml
- filename: opkey-generic-api-openapi.yml
  format: yaml
  label: Opkey Generic API
  slug: opkey-generic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-generic-api-openapi.yml
- filename: opkey-network-simulation-api-openapi.yml
  format: yaml
  label: Opkey Network Simulation API
  slug: opkey-network-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-network-simulation-api-openapi.yml
- filename: opkey-performance-api-openapi.yml
  format: yaml
  label: Opkey Performance API
  slug: opkey-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-performance-api-openapi.yml
- filename: opkey-resigning-apis-api-openapi.yml
  format: yaml
  label: Opkey Resigning Apis API
  slug: opkey-resigning-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-resigning-apis-api-openapi.yml
- filename: opkey-session-media-logs-api-openapi.yml
  format: yaml
  label: Opkey Session Media & Logs API
  slug: opkey-session-media-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-session-media-logs-api-openapi.yml
- filename: opkey-xctest-automation-api-openapi.yml
  format: yaml
  label: Opkey Xctest Automation API
  slug: opkey-xctest-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-xctest-automation-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: opkey.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pcloudy.com
  spf: true
hosts:
- cert_expires: Sep 27 05:46:03 2026 GMT
  host: www.opkey.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: www.pcloudy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: device.pcloudy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opkey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opkey, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Opkey
provider_slug: opkey
slug: opkey-domain-security
source_filename: opkey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opkey.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 05:46:03 2026 GMT\n  hsts: null\n- host: www.pcloudy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: false\n- host: device.pcloudy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opkey.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: pcloudy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/security/opkey-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Testing
- Test Automation
- Quality Assurance
- DevOps
- Continuous Integration
- Mobile Testing
- Device Cloud
- ERP
- Artificial Intelligence
- Agents
- MCP
---
