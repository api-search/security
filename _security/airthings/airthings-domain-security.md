---
api_specs:
- filename: airthings-accounts-api-openapi.yml
  format: yaml
  label: Airthings Accounts API
  slug: airthings-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-accounts-api-openapi.yml
- filename: airthings-device-api-openapi.yml
  format: yaml
  label: Airthings Device API
  slug: airthings-device-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-device-api-openapi.yml
- filename: airthings-devices-api-openapi.yml
  format: yaml
  label: Airthings Devices API
  slug: airthings-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-devices-api-openapi.yml
- filename: airthings-health-api-openapi.yml
  format: yaml
  label: Airthings Health API
  slug: airthings-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-health-api-openapi.yml
- filename: airthings-locations-api-openapi.yml
  format: yaml
  label: Airthings Locations API
  slug: airthings-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-locations-api-openapi.yml
- filename: airthings-organizations-api-openapi.yml
  format: yaml
  label: Airthings Organizations API
  slug: airthings-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-organizations-api-openapi.yml
- filename: airthings-segments-api-openapi.yml
  format: yaml
  label: Airthings Segments API
  slug: airthings-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-segments-api-openapi.yml
- filename: airthings-sensor-api-openapi.yml
  format: yaml
  label: Airthings Sensor API
  slug: airthings-sensor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-sensor-api-openapi.yml
- filename: airthings-spaces-api-openapi.yml
  format: yaml
  label: Airthings Spaces API
  slug: airthings-spaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-spaces-api-openapi.yml
- filename: airthings-thresholds-api-openapi.yml
  format: yaml
  label: Airthings Thresholds API
  slug: airthings-thresholds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-thresholds-api-openapi.yml
- filename: airthings-webhooks-api-openapi.yml
  format: yaml
  label: Airthings Webhooks API
  slug: airthings-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: airthings.com
  spf: true
hosts:
- cert_expires: May  4 23:59:59 2027 GMT
  host: airthings.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Airthings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airthings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Airthings
provider_slug: airthings
slug: airthings-domain-security
source_filename: airthings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airthings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: airthings.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/airthings/security/airthings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AirQuality
- Radon
- Sensors
- IoT
---
