---
api_specs:
- filename: cyclr-account-connector-custom-categories-api-openapi.yml
  format: yaml
  label: Cyclr Account Connector Custom Categories API
  slug: cyclr-account-connector-custom-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-account-connector-custom-categories-api-openapi.yml
- filename: cyclr-account-connector-properties-api-openapi.yml
  format: yaml
  label: Cyclr Account Connector Properties API
  slug: cyclr-account-connector-properties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-account-connector-properties-api-openapi.yml
- filename: cyclr-account-connectors-api-openapi.yml
  format: yaml
  label: Cyclr Account Connectors API
  slug: cyclr-account-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-account-connectors-api-openapi.yml
- filename: cyclr-account-custom-connectors-api-openapi.yml
  format: yaml
  label: Cyclr Account Custom Connectors API
  slug: cyclr-account-custom-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-account-custom-connectors-api-openapi.yml
- filename: cyclr-accounts-api-openapi.yml
  format: yaml
  label: Cyclr Accounts API
  slug: cyclr-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-accounts-api-openapi.yml
- filename: cyclr-authentication-api-openapi.yml
  format: yaml
  label: Cyclr Authentication API
  slug: cyclr-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-authentication-api-openapi.yml
- filename: cyclr-connectors-api-openapi.yml
  format: yaml
  label: Cyclr Connectors API
  slug: cyclr-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-connectors-api-openapi.yml
- filename: cyclr-custom-fields-api-openapi.yml
  format: yaml
  label: Cyclr Custom Fields API
  slug: cyclr-custom-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-custom-fields-api-openapi.yml
- filename: cyclr-cycles-api-openapi.yml
  format: yaml
  label: Cyclr Cycles API
  slug: cyclr-cycles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-cycles-api-openapi.yml
- filename: cyclr-edges-api-openapi.yml
  format: yaml
  label: Cyclr Edges API
  slug: cyclr-edges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-edges-api-openapi.yml
- filename: cyclr-mcp-servers-api-openapi.yml
  format: yaml
  label: Cyclr MCP Servers API
  slug: cyclr-mcp-servers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-mcp-servers-api-openapi.yml
- filename: cyclr-methods-api-openapi.yml
  format: yaml
  label: Cyclr Methods API
  slug: cyclr-methods-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-methods-api-openapi.yml
- filename: cyclr-steps-api-openapi.yml
  format: yaml
  label: Cyclr Steps API
  slug: cyclr-steps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-steps-api-openapi.yml
- filename: cyclr-templates-api-openapi.yml
  format: yaml
  label: Cyclr Templates API
  slug: cyclr-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-templates-api-openapi.yml
- filename: cyclr-transactions-api-openapi.yml
  format: yaml
  label: Cyclr Transactions API
  slug: cyclr-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-transactions-api-openapi.yml
- filename: cyclr-users-api-openapi.yml
  format: yaml
  label: Cyclr Users API
  slug: cyclr-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: cyclr.com
  spf: true
hosts:
- cert_expires: Jan  1 23:49:19 2027 GMT
  host: cyclr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 29 23:59:59 2027 GMT
  host: api.cyclr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Cyclr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cyclr, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cyclr
provider_slug: cyclr
slug: cyclr-domain-security
source_filename: cyclr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cyclr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:49:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cyclr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 29 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: cyclr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/cyclr/security/cyclr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Connectors
- Custom Connectors
- Data Synchronization
- Embedded iPaaS
- Embedded SaaS Integration
- Embedded UI
- Integration Platform
- Integration
- Marketplace
- Authentication
- REST API
- Software-as-a-Service
- Templates
- Webhook
- White Label
- Workflows
---
