---
api_specs:
- filename: evcc-auth-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Auth API
  slug: evcc-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-auth-api-openapi.yml
- filename: evcc-battery-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Battery API
  slug: evcc-battery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-battery-api-openapi.yml
- filename: evcc-db-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Db API
  slug: evcc-db-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-db-api-openapi.yml
- filename: evcc-experimental-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Experimental API
  slug: evcc-experimental-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-experimental-api-openapi.yml
- filename: evcc-general-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) General API
  slug: evcc-general-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-general-api-openapi.yml
- filename: evcc-loadpoints-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Loadpoints API
  slug: evcc-loadpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-loadpoints-api-openapi.yml
- filename: evcc-sessions-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Sessions API
  slug: evcc-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-sessions-api-openapi.yml
- filename: evcc-state-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) State API
  slug: evcc-state-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-state-api-openapi.yml
- filename: evcc-system-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) System API
  slug: evcc-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-system-api-openapi.yml
- filename: evcc-tariffs-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Tariffs API
  slug: evcc-tariffs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-tariffs-api-openapi.yml
- filename: evcc-vehicles-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Vehicles API
  slug: evcc-vehicles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-vehicles-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: evcc.io
  spf: false
hosts:
- cert_expires: Jan 16 07:34:48 2027 GMT
  host: evcc.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Evcc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for evcc (self-hosted), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: evcc (self-hosted)
provider_slug: evcc
slug: evcc-domain-security
source_filename: evcc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: evcc.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 07:34:48 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: evcc.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/evcc/security/evcc-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- EV
- SmartCharging
- OpenSource
- EnergyManagement
- HomeAutomation
---
