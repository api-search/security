---
api_specs:
- filename: bright-sky-alerts-api-openapi.yml
  format: yaml
  label: Bright Sky Alerts API
  slug: bright-sky-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bright-sky/openapi/bright-sky-alerts-api-openapi.yml
- filename: bright-sky-current-weather-api-openapi.yml
  format: yaml
  label: Bright Sky Current Weather API
  slug: bright-sky-current-weather-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bright-sky/openapi/bright-sky-current-weather-api-openapi.yml
- filename: bright-sky-internals-api-openapi.yml
  format: yaml
  label: Bright Sky Internals API
  slug: bright-sky-internals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bright-sky/openapi/bright-sky-internals-api-openapi.yml
- filename: bright-sky-radar-api-openapi.yml
  format: yaml
  label: Bright Sky Radar API
  slug: bright-sky-radar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bright-sky/openapi/bright-sky-radar-api-openapi.yml
- filename: bright-sky-weather-api-openapi.yml
  format: yaml
  label: Bright Sky Weather API
  slug: bright-sky-weather-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bright-sky/openapi/bright-sky-weather-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: brightsky.dev
  spf: true
hosts:
- cert_expires: Jan 22 11:29:23 2027 GMT
  host: brightsky.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bright Sky Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bright Sky, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bright Sky
provider_slug: bright-sky
slug: bright-sky-domain-security
source_filename: bright-sky-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brightsky.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 11:29:23 2027 GMT\n  hsts: false\ndomains:\n- domain: brightsky.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/bright-sky/security/bright-sky-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Weather
- API
- OpenData
- JSON
---
