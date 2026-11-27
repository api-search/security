---
api_specs:
- filename: milemaker-com-asset-trace-management-api-openapi.yml
  format: yaml
  label: MileMaker Asset Trace Management API
  slug: milemaker-com-asset-trace-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/milemaker-com/openapi/milemaker-com-asset-trace-management-api-openapi.yml
- filename: milemaker-com-avoidareas-api-openapi.yml
  format: yaml
  label: MileMaker Avoid Areas API
  slug: milemaker-com-avoidareas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/milemaker-com/openapi/milemaker-com-avoidareas-api-openapi.yml
- filename: milemaker-com-cached-route-plan-api-openapi.yml
  format: yaml
  label: MileMaker Cached Route Plan API
  slug: milemaker-com-cached-route-plan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/milemaker-com/openapi/milemaker-com-cached-route-plan-api-openapi.yml
- filename: milemaker-com-content-api-openapi.yml
  format: yaml
  label: MileMaker Content API
  slug: milemaker-com-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/milemaker-com/openapi/milemaker-com-content-api-openapi.yml
- filename: milemaker-com-locations-api-openapi.yml
  format: yaml
  label: MileMaker Locations API
  slug: milemaker-com-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/milemaker-com/openapi/milemaker-com-locations-api-openapi.yml
- filename: milemaker-com-route-planning-api-openapi.yml
  format: yaml
  label: MileMaker Route Planning API
  slug: milemaker-com-route-planning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/milemaker-com/openapi/milemaker-com-route-planning-api-openapi.yml
- filename: milemaker-com-route-reconstruction-api-openapi.yml
  format: yaml
  label: MileMaker Route Reconstruction API
  slug: milemaker-com-route-reconstruction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/milemaker-com/openapi/milemaker-com-route-reconstruction-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: milemaker.com
  spf: true
hosts:
- cert_expires: Feb 10 00:02:40 2027 GMT
  host: milemaker.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MileMaker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MileMaker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MileMaker
provider_slug: milemaker-com
slug: milemaker-com-domain-security
source_filename: milemaker-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: milemaker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 00:02:40 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: milemaker.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/milemaker-com/security/milemaker-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Logistics
- Transportation
- Routing
- Mileage
- Trucking
---
