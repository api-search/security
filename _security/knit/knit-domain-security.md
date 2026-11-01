---
api_specs:
- filename: knit-departments-api-openapi.yml
  format: yaml
  label: Knit Departments API
  slug: knit-departments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knit/openapi/knit-departments-api-openapi.yml
- filename: knit-employees-api-openapi.yml
  format: yaml
  label: Knit Employees API
  slug: knit-employees-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knit/openapi/knit-employees-api-openapi.yml
- filename: knit-integrations-api-openapi.yml
  format: yaml
  label: Knit Integrations API
  slug: knit-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knit/openapi/knit-integrations-api-openapi.yml
- filename: knit-jobs-api-openapi.yml
  format: yaml
  label: Knit Jobs API
  slug: knit-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knit/openapi/knit-jobs-api-openapi.yml
- filename: knit-locations-api-openapi.yml
  format: yaml
  label: Knit Locations API
  slug: knit-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knit/openapi/knit-locations-api-openapi.yml
- filename: knit-syncs-api-openapi.yml
  format: yaml
  label: Knit Syncs API
  slug: knit-syncs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knit/openapi/knit-syncs-api-openapi.yml
- filename: knit-time-off-api-openapi.yml
  format: yaml
  label: Knit Time Off API
  slug: knit-time-off-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knit/openapi/knit-time-off-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getknit.dev
  spf: true
hosts:
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: www.getknit.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 08:24:54 2026 GMT
  host: developers.getknit.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr 17 23:59:59 2027 GMT
  host: api.getknit.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Knit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knit, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Knit
provider_slug: knit
slug: knit-domain-security
source_filename: knit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getknit.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: false\n- host: developers.getknit.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 08:24:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getknit.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: getknit.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/knit/security/knit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B
- HR Integrations
- HRIS
- Unified API
- Integration Platform
- API Management
- iPaaS
- Automation
- SaaS Integration
- AI Agents
---
