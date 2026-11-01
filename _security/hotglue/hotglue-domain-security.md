---
api_specs:
- filename: hotglue-jobs-api-openapi.yml
  format: yaml
  label: Hotglue Jobs API
  slug: hotglue-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-jobs-api-openapi.yml
- filename: hotglue-availableconnectors-api-openapi.yml
  format: yaml
  label: Hotglue Available Connectors API
  slug: hotglue-availableconnectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-availableconnectors-api-openapi.yml
- filename: hotglue-availablesources-api-openapi.yml
  format: yaml
  label: Hotglue Available Sources API
  slug: hotglue-availablesources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-availablesources-api-openapi.yml
- filename: hotglue-availabletargets-api-openapi.yml
  format: yaml
  label: Hotglue Available Targets API
  slug: hotglue-availabletargets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-availabletargets-api-openapi.yml
- filename: hotglue-connectors-api-openapi.yml
  format: yaml
  label: Hotglue Connectors API
  slug: hotglue-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-connectors-api-openapi.yml
- filename: hotglue-flows-api-openapi.yml
  format: yaml
  label: Hotglue Flows API
  slug: hotglue-flows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-flows-api-openapi.yml
- filename: hotglue-jupyter-api-openapi.yml
  format: yaml
  label: Hotglue Jupyter API
  slug: hotglue-jupyter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-jupyter-api-openapi.yml
- filename: hotglue-linkedconnectors-api-openapi.yml
  format: yaml
  label: Hotglue Linked Connectors API
  slug: hotglue-linkedconnectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-linkedconnectors-api-openapi.yml
- filename: hotglue-linkedsources-api-openapi.yml
  format: yaml
  label: Hotglue Linked Sources API
  slug: hotglue-linkedsources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-linkedsources-api-openapi.yml
- filename: hotglue-linkedtargets-api-openapi.yml
  format: yaml
  label: Hotglue Linked Targets API
  slug: hotglue-linkedtargets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-linkedtargets-api-openapi.yml
- filename: hotglue-mcptoken-api-openapi.yml
  format: yaml
  label: Hotglue MCP Token API
  slug: hotglue-mcptoken-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-mcptoken-api-openapi.yml
- filename: hotglue-supportedconnectors-api-openapi.yml
  format: yaml
  label: Hotglue Supported Connectors API
  slug: hotglue-supportedconnectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-supportedconnectors-api-openapi.yml
- filename: hotglue-supportedsources-api-openapi.yml
  format: yaml
  label: Hotglue Supported Sources API
  slug: hotglue-supportedsources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-supportedsources-api-openapi.yml
- filename: hotglue-supportedtargets-api-openapi.yml
  format: yaml
  label: Hotglue Supported Targets API
  slug: hotglue-supportedtargets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-supportedtargets-api-openapi.yml
- filename: hotglue-tenant-api-openapi.yml
  format: yaml
  label: Hotglue Tenant API
  slug: hotglue-tenant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-tenant-api-openapi.yml
- filename: hotglue-tenants-api-openapi.yml
  format: yaml
  label: Hotglue Tenants API
  slug: hotglue-tenants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-tenants-api-openapi.yml
- filename: hotglue-magic-link-api-openapi.yml
  format: yaml
  label: Hotglue Magic Link API
  slug: hotglue-magic-link-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-magic-link-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hotglue.com
  spf: true
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: hotglue.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 18:51:37 2026 GMT
  host: docs.hotglue.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: api.hotglue.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Hotglue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hotglue, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hotglue
provider_slug: hotglue
slug: hotglue-domain-security
source_filename: hotglue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hotglue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: false\n- host: docs.hotglue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 18:51:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.hotglue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hotglue.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/hotglue/security/hotglue-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Connectors
- Embedded Integrations
- ETL
- Integration Platform
- iPaaS
---
