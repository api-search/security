---
api_specs:
- filename: startup-jobs-companies-api-openapi.yml
  format: yaml
  label: startup-jobs Companies API
  slug: startup-jobs-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/startup-jobs/openapi/startup-jobs-companies-api-openapi.yml
- filename: startup-jobs-jobs-api-openapi.yml
  format: yaml
  label: startup-jobs Jobs API
  slug: startup-jobs-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/startup-jobs/openapi/startup-jobs-jobs-api-openapi.yml
- filename: startup-jobs-locations-api-openapi.yml
  format: yaml
  label: startup-jobs Locations API
  slug: startup-jobs-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/startup-jobs/openapi/startup-jobs-locations-api-openapi.yml
- filename: startup-jobs-openapi-json-api-openapi.yml
  format: yaml
  label: startup-jobs Openapi.json API
  slug: startup-jobs-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/startup-jobs/openapi/startup-jobs-openapi-json-api-openapi.yml
- filename: startup-jobs-roles-api-openapi.yml
  format: yaml
  label: startup-jobs Roles API
  slug: startup-jobs-roles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/startup-jobs/openapi/startup-jobs-roles-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: startup.jobs
  spf: true
hosts:
- cert_expires: Dec 15 10:47:53 2026 GMT
  host: startup.jobs
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Startup Jobs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for startup-jobs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: startup-jobs
provider_slug: startup-jobs
slug: startup-jobs-domain-security
source_filename: startup-jobs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: startup.jobs\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 10:47:53 2026 GMT\n  hsts: null\ndomains:\n- domain: startup.jobs\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/startup-jobs/security/startup-jobs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
