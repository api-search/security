---
api_specs:
- filename: enode-batteries-api-openapi.yml
  format: yaml
  label: Enode Batteries API
  slug: enode-batteries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-batteries-api-openapi.yml
- filename: enode-chargers-api-openapi.yml
  format: yaml
  label: Enode Chargers API
  slug: enode-chargers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-chargers-api-openapi.yml
- filename: enode-hvac-api-openapi.yml
  format: yaml
  label: Enode HVAC API
  slug: enode-hvac-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-hvac-api-openapi.yml
- filename: enode-meters-api-openapi.yml
  format: yaml
  label: Enode Meters API
  slug: enode-meters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-meters-api-openapi.yml
- filename: enode-vehicles-api-openapi.yml
  format: yaml
  label: Enode Vehicles API
  slug: enode-vehicles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-vehicles-api-openapi.yml
- filename: enode-webhooks-api-openapi.yml
  format: yaml
  label: Enode Webhooks API
  slug: enode-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-webhooks-api-openapi.yml
- filename: enode-beta-api-openapi.yml
  format: yaml
  label: Enode Beta API
  slug: enode-beta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-beta-api-openapi.yml
- filename: enode-early-adopter-api-openapi.yml
  format: yaml
  label: Enode Early Adopter API
  slug: enode-early-adopter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-early-adopter-api-openapi.yml
- filename: enode-interventions-api-openapi.yml
  format: yaml
  label: Enode Interventions API
  slug: enode-interventions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-interventions-api-openapi.yml
- filename: enode-locations-api-openapi.yml
  format: yaml
  label: Enode Locations API
  slug: enode-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-locations-api-openapi.yml
- filename: enode-schedules-api-openapi.yml
  format: yaml
  label: Enode Schedules API
  slug: enode-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-schedules-api-openapi.yml
- filename: enode-service-health-api-openapi.yml
  format: yaml
  label: Enode Service Health API
  slug: enode-service-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-service-health-api-openapi.yml
- filename: enode-solar-inverters-api-openapi.yml
  format: yaml
  label: Enode Solar inverters API
  slug: enode-solar-inverters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-solar-inverters-api-openapi.yml
- filename: enode-statistics-api-openapi.yml
  format: yaml
  label: Enode Statistics API
  slug: enode-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-statistics-api-openapi.yml
- filename: enode-tariffs-api-openapi.yml
  format: yaml
  label: Enode Tariffs API
  slug: enode-tariffs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-tariffs-api-openapi.yml
- filename: enode-user-management-api-openapi.yml
  format: yaml
  label: Enode User Management API
  slug: enode-user-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enode/openapi/enode-user-management-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: enode.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: enode.io
  spf: false
hosts:
- cert_expires: Sep  2 13:20:53 2026 GMT
  host: www.enode.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 04:56:20 2026 GMT
  host: developers.enode.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: enode-api.production.enode.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Enode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enode, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Enode
provider_slug: enode
slug: enode-domain-security
source_filename: enode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.enode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 13:20:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.enode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 04:56:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: enode-api.production.enode.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: enode.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: enode.io\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/enode/security/enode-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- Electric Vehicles
- EV Charging
- Smart Charging
- Energy Transition
- Mobility
---
