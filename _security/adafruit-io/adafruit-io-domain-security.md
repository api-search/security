---
api_specs:
- filename: adafruit-io-activities-api-openapi.yml
  format: yaml
  label: Adafruit IO Activities API
  slug: adafruit-io-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/openapi/adafruit-io-activities-api-openapi.yml
- filename: adafruit-io-blocks-api-openapi.yml
  format: yaml
  label: Adafruit IO Blocks API
  slug: adafruit-io-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/openapi/adafruit-io-blocks-api-openapi.yml
- filename: adafruit-io-dashboards-api-openapi.yml
  format: yaml
  label: Adafruit IO Dashboards API
  slug: adafruit-io-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/openapi/adafruit-io-dashboards-api-openapi.yml
- filename: adafruit-io-data-api-openapi.yml
  format: yaml
  label: Adafruit IO Data API
  slug: adafruit-io-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/openapi/adafruit-io-data-api-openapi.yml
- filename: adafruit-io-feeds-api-openapi.yml
  format: yaml
  label: Adafruit IO Feeds API
  slug: adafruit-io-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/openapi/adafruit-io-feeds-api-openapi.yml
- filename: adafruit-io-groups-api-openapi.yml
  format: yaml
  label: Adafruit IO Groups API
  slug: adafruit-io-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/openapi/adafruit-io-groups-api-openapi.yml
- filename: adafruit-io-permissions-api-openapi.yml
  format: yaml
  label: Adafruit IO Permissions API
  slug: adafruit-io-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/openapi/adafruit-io-permissions-api-openapi.yml
- filename: adafruit-io-tokens-api-openapi.yml
  format: yaml
  label: Adafruit IO Tokens API
  slug: adafruit-io-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/openapi/adafruit-io-tokens-api-openapi.yml
- filename: adafruit-io-triggers-api-openapi.yml
  format: yaml
  label: Adafruit IO Triggers API
  slug: adafruit-io-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/openapi/adafruit-io-triggers-api-openapi.yml
- filename: adafruit-io-users-api-openapi.yml
  format: yaml
  label: Adafruit IO Users API
  slug: adafruit-io-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/openapi/adafruit-io-users-api-openapi.yml
- filename: adafruit-io-webhooks-api-openapi.yml
  format: yaml
  label: Adafruit IO Webhooks API
  slug: adafruit-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/openapi/adafruit-io-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: adafruit.com
  spf: true
hosts:
- cert_expires: Aug  3 23:59:59 2026 GMT
  host: io.adafruit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adafruit Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adafruit IO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Adafruit IO
provider_slug: adafruit-io
slug: adafruit-io-domain-security
source_filename: adafruit-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: io.adafruit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: adafruit.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/security/adafruit-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- IoT
- Internet of Things
- MQTT
- Maker
- Hobbyist
- CircuitPython
- Arduino
- ESP32
- Feather
- Dashboards
- Time Series
---
