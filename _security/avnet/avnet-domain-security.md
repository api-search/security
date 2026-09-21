---
api_specs:
- filename: avnet-iotconnect-master-openapi.yml
  format: yaml
  label: Avnet /IOTCONNECT Master API
  slug: avnet-iotconnect-master-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avnet/refs/heads/main/openapi/avnet-iotconnect-master-openapi.yml
- filename: avnet-iotconnect-auth-openapi.yml
  format: yaml
  label: Avnet /IOTCONNECT Authenticate API
  slug: avnet-iotconnect-authenticate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avnet/refs/heads/main/openapi/avnet-iotconnect-auth-openapi.yml
- filename: avnet-iotconnect-user-openapi.yml
  format: yaml
  label: Avnet /IOTCONNECT User API
  slug: avnet-iotconnect-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avnet/refs/heads/main/openapi/avnet-iotconnect-user-openapi.yml
- filename: avnet-iotconnect-device-openapi.yml
  format: yaml
  label: Avnet /IOTCONNECT Device API
  slug: avnet-iotconnect-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avnet/refs/heads/main/openapi/avnet-iotconnect-device-openapi.yml
- filename: avnet-iotconnect-firmware-openapi.yml
  format: yaml
  label: Avnet /IOTCONNECT Firmware API
  slug: avnet-iotconnect-firmware-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avnet/refs/heads/main/openapi/avnet-iotconnect-firmware-openapi.yml
- filename: avnet-iotconnect-event-openapi.yml
  format: yaml
  label: Avnet /IOTCONNECT Event API
  slug: avnet-iotconnect-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avnet/refs/heads/main/openapi/avnet-iotconnect-event-openapi.yml
- filename: avnet-iotconnect-telemetry-openapi.yml
  format: yaml
  label: Avnet /IOTCONNECT Telemetry API
  slug: avnet-iotconnect-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avnet/refs/heads/main/openapi/avnet-iotconnect-telemetry-openapi.yml
- filename: avnet-iotconnect-file-openapi.yml
  format: yaml
  label: Avnet /IOTCONNECT File API
  slug: avnet-iotconnect-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avnet/refs/heads/main/openapi/avnet-iotconnect-file-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: avnet.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.avnet.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: apiportal.avnet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: apigw.avnet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Avnet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avnet, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Avnet
provider_slug: avnet
slug: avnet-domain-security
source_filename: avnet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avnet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: apiportal.avnet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apigw.avnet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: avnet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avnet/refs/heads/main/security/avnet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
- Electronics
- Components
- Supply Chain
- IoT
- Manufacturing
- Distribution
- Procurement
- Device Management
- Firmware
---
