---
api_specs:
- filename: teslemetry-automations-api-openapi.yml
  format: yaml
  label: Teslemetry Automations API
  slug: teslemetry-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslemetry/openapi/teslemetry-automations-api-openapi.yml
- filename: teslemetry-charging-api-openapi.yml
  format: yaml
  label: Teslemetry Charging API
  slug: teslemetry-charging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslemetry/openapi/teslemetry-charging-api-openapi.yml
- filename: teslemetry-energy-api-openapi.yml
  format: yaml
  label: Teslemetry Energy API
  slug: teslemetry-energy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslemetry/openapi/teslemetry-energy-api-openapi.yml
- filename: teslemetry-energy-command-api-openapi.yml
  format: yaml
  label: Teslemetry Energy Command API
  slug: teslemetry-energy-command-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslemetry/openapi/teslemetry-energy-command-api-openapi.yml
- filename: teslemetry-general-api-openapi.yml
  format: yaml
  label: Teslemetry General API
  slug: teslemetry-general-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslemetry/openapi/teslemetry-general-api-openapi.yml
- filename: teslemetry-meta-api-openapi.yml
  format: yaml
  label: Teslemetry Meta API
  slug: teslemetry-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslemetry/openapi/teslemetry-meta-api-openapi.yml
- filename: teslemetry-streaming-api-openapi.yml
  format: yaml
  label: Teslemetry Streaming API
  slug: teslemetry-streaming-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslemetry/openapi/teslemetry-streaming-api-openapi.yml
- filename: teslemetry-user-api-openapi.yml
  format: yaml
  label: Teslemetry User API
  slug: teslemetry-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslemetry/openapi/teslemetry-user-api-openapi.yml
- filename: teslemetry-vehicle-api-openapi.yml
  format: yaml
  label: Teslemetry Vehicle API
  slug: teslemetry-vehicle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslemetry/openapi/teslemetry-vehicle-api-openapi.yml
- filename: teslemetry-vehicle-command-api-openapi.yml
  format: yaml
  label: Teslemetry Vehicle Command API
  slug: teslemetry-vehicle-command-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslemetry/openapi/teslemetry-vehicle-command-api-openapi.yml
- filename: teslemetry-vehicle-custom-commands-api-openapi.yml
  format: yaml
  label: Teslemetry Vehicle Custom Commands API
  slug: teslemetry-vehicle-custom-commands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslemetry/openapi/teslemetry-vehicle-custom-commands-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: teslemetry.com
  spf: true
hosts:
- cert_expires: Jan 24 12:12:11 2027 GMT
  host: teslemetry.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Teslemetry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teslemetry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Teslemetry
provider_slug: teslemetry
slug: teslemetry-domain-security
source_filename: teslemetry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: teslemetry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 12:12:11 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: teslemetry.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/teslemetry/security/teslemetry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Tesla
- Fleet API
- Home Automation
- Energy
---
