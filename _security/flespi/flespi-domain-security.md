---
api_specs:
- filename: flespi-assets-api-openapi.yml
  format: yaml
  label: flespi Assets API
  slug: flespi-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flespi/openapi/flespi-assets-api-openapi.yml
- filename: flespi-calculators-api-openapi.yml
  format: yaml
  label: flespi Calculators API
  slug: flespi-calculators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flespi/openapi/flespi-calculators-api-openapi.yml
- filename: flespi-changelog-api-openapi.yml
  format: yaml
  label: flespi Changelog API
  slug: flespi-changelog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flespi/openapi/flespi-changelog-api-openapi.yml
- filename: flespi-channels-api-openapi.yml
  format: yaml
  label: flespi Channels API
  slug: flespi-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flespi/openapi/flespi-channels-api-openapi.yml
- filename: flespi-devices-api-openapi.yml
  format: yaml
  label: flespi Devices API
  slug: flespi-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flespi/openapi/flespi-devices-api-openapi.yml
- filename: flespi-geofences-api-openapi.yml
  format: yaml
  label: flespi Geofences API
  slug: flespi-geofences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flespi/openapi/flespi-geofences-api-openapi.yml
- filename: flespi-groups-api-openapi.yml
  format: yaml
  label: flespi Groups API
  slug: flespi-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flespi/openapi/flespi-groups-api-openapi.yml
- filename: flespi-modems-api-openapi.yml
  format: yaml
  label: flespi Modems API
  slug: flespi-modems-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flespi/openapi/flespi-modems-api-openapi.yml
- filename: flespi-plugins-api-openapi.yml
  format: yaml
  label: flespi Plugins API
  slug: flespi-plugins-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flespi/openapi/flespi-plugins-api-openapi.yml
- filename: flespi-protocols-api-openapi.yml
  format: yaml
  label: flespi Protocols API
  slug: flespi-protocols-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flespi/openapi/flespi-protocols-api-openapi.yml
- filename: flespi-streams-api-openapi.yml
  format: yaml
  label: flespi Streams API
  slug: flespi-streams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flespi/openapi/flespi-streams-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flespi.com
  spf: true
hosts:
- cert_expires: Dec 12 13:40:46 2026 GMT
  host: flespi.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: flespi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for flespi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: flespi
provider_slug: flespi
slug: flespi-domain-security
source_filename: flespi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flespi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 13:40:46 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: flespi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/flespi/security/flespi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telematics
- IoT
- Data Ingestion
- Real-Time Analytics
---
