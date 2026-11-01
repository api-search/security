---
api_specs:
- filename: home-connect-appliances-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Appliances API
  slug: home-connect-appliances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-appliances-api-openapi.yml
- filename: home-connect-commands-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Commands API
  slug: home-connect-commands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-commands-api-openapi.yml
- filename: home-connect-events-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Events API
  slug: home-connect-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-events-api-openapi.yml
- filename: home-connect-images-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Images API
  slug: home-connect-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-images-api-openapi.yml
- filename: home-connect-map-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Map API
  slug: home-connect-map-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-map-api-openapi.yml
- filename: home-connect-programs-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Programs API
  slug: home-connect-programs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-programs-api-openapi.yml
- filename: home-connect-settings-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Settings API
  slug: home-connect-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-settings-api-openapi.yml
- filename: home-connect-status-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Status API
  slug: home-connect-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: home-connect.com
  spf: true
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: home-connect.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Home Connect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Home Connect (BSH appliances), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Home Connect (BSH appliances)
provider_slug: home-connect
slug: home-connect-domain-security
source_filename: home-connect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: home-connect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: home-connect.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/home-connect/security/home-connect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- smart home
- appliances
- connected devices
---
