---
api_specs:
- filename: arrivy-entity-apis-api-openapi.yml
  format: yaml
  label: Arrivy Entity APIs API
  slug: arrivy-entity-apis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arrivy/openapi/arrivy-entity-apis-api-openapi.yml
- filename: arrivy-location-report-apis-api-openapi.yml
  format: yaml
  label: Arrivy Location Report APIs API
  slug: arrivy-location-report-apis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arrivy/openapi/arrivy-location-report-apis-api-openapi.yml
- filename: arrivy-task-apis-api-openapi.yml
  format: yaml
  label: Arrivy Task APIs API
  slug: arrivy-task-apis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arrivy/openapi/arrivy-task-apis-api-openapi.yml
- filename: arrivy-task-status-apis-api-openapi.yml
  format: yaml
  label: Arrivy Task Status APIs API
  slug: arrivy-task-status-apis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arrivy/openapi/arrivy-task-status-apis-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arrivy.com
  spf: true
hosts:
- cert_expires: Jan 23 23:03:36 2027 GMT
  host: arrivy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arrivy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arrivy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Arrivy
provider_slug: arrivy
slug: arrivy-domain-security
source_filename: arrivy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arrivy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:03:36 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arrivy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/arrivy/security/arrivy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Field Service Management
- Operations Software
- Cloud Platform
- Integration
---
