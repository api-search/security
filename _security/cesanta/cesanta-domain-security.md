---
api_specs:
- filename: cesanta-data-api-openapi.yml
  format: yaml
  label: Cesanta Data API
  slug: cesanta-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cesanta/refs/heads/main/openapi/cesanta-data-api-openapi.yml
- filename: cesanta-devices-api-openapi.yml
  format: yaml
  label: Cesanta Devices API
  slug: cesanta-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cesanta/refs/heads/main/openapi/cesanta-devices-api-openapi.yml
- filename: cesanta-keys-api-openapi.yml
  format: yaml
  label: Cesanta Keys API
  slug: cesanta-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cesanta/refs/heads/main/openapi/cesanta-keys-api-openapi.yml
- filename: cesanta-logs-api-openapi.yml
  format: yaml
  label: Cesanta Logs API
  slug: cesanta-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cesanta/refs/heads/main/openapi/cesanta-logs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cesanta.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: mdash.net
  spf: false
hosts:
- cert_expires: Sep 21 12:51:20 2026 GMT
  host: cesanta.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 07:07:59 2026 GMT
  host: mdash.net
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  6 07:07:59 2026 GMT
  host: dash.mongoose-os.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cesanta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cesanta, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cesanta
provider_slug: cesanta
slug: cesanta-domain-security
source_filename: cesanta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cesanta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 12:51:20 2026 GMT\n  hsts: false\n- host: mdash.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  6 07:07:59 2026 GMT\n  hsts: null\n- host: dash.mongoose-os.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  6 07:07:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cesanta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mdash.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cesanta/refs/heads/main/security/cesanta-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- IoT
- Embedded
- Device Management
- Firmware
- OTA
- Networking
- MQTT
---
