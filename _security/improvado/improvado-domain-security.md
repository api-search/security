---
api_specs:
- filename: improvado-accounts-api-openapi.yml
  format: yaml
  label: Improvado Accounts API
  slug: improvado-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/improvado/openapi/improvado-accounts-api-openapi.yml
- filename: improvado-authentication-api-openapi.yml
  format: yaml
  label: Improvado Authentication API
  slug: improvado-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/improvado/openapi/improvado-authentication-api-openapi.yml
- filename: improvado-automated-recipes-api-openapi.yml
  format: yaml
  label: Improvado Automated Recipes API
  slug: improvado-automated-recipes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/improvado/openapi/improvado-automated-recipes-api-openapi.yml
- filename: improvado-data-source-connections-api-openapi.yml
  format: yaml
  label: Improvado Data source connections API
  slug: improvado-data-source-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/improvado/openapi/improvado-data-source-connections-api-openapi.yml
- filename: improvado-data-sources-api-openapi.yml
  format: yaml
  label: Improvado Data sources API
  slug: improvado-data-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/improvado/openapi/improvado-data-sources-api-openapi.yml
- filename: improvado-data-tables-api-openapi.yml
  format: yaml
  label: Improvado Data tables API
  slug: improvado-data-tables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/improvado/openapi/improvado-data-tables-api-openapi.yml
- filename: improvado-destination-connections-api-openapi.yml
  format: yaml
  label: Improvado Destination connections API
  slug: improvado-destination-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/improvado/openapi/improvado-destination-connections-api-openapi.yml
- filename: improvado-destinations-api-openapi.yml
  format: yaml
  label: Improvado Destinations API
  slug: improvado-destinations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/improvado/openapi/improvado-destinations-api-openapi.yml
- filename: improvado-extraction-templates-api-openapi.yml
  format: yaml
  label: Improvado Extraction templates API
  slug: improvado-extraction-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/improvado/openapi/improvado-extraction-templates-api-openapi.yml
- filename: improvado-extracts-api-openapi.yml
  format: yaml
  label: Improvado Extracts API
  slug: improvado-extracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/improvado/openapi/improvado-extracts-api-openapi.yml
- filename: improvado-iframe-api-openapi.yml
  format: yaml
  label: Improvado Iframe API
  slug: improvado-iframe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/improvado/openapi/improvado-iframe-api-openapi.yml
- filename: improvado-loads-api-openapi.yml
  format: yaml
  label: Improvado Loads API
  slug: improvado-loads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/improvado/openapi/improvado-loads-api-openapi.yml
- filename: improvado-recipes-api-openapi.yml
  format: yaml
  label: Improvado Recipes API
  slug: improvado-recipes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/improvado/openapi/improvado-recipes-api-openapi.yml
- filename: improvado-roles-api-openapi.yml
  format: yaml
  label: Improvado Roles API
  slug: improvado-roles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/improvado/openapi/improvado-roles-api-openapi.yml
- filename: improvado-webhooks-api-openapi.yml
  format: yaml
  label: Improvado Webhooks API
  slug: improvado-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/improvado/openapi/improvado-webhooks-api-openapi.yml
- filename: improvado-workspaces-api-openapi.yml
  format: yaml
  label: Improvado Workspaces API
  slug: improvado-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/improvado/openapi/improvado-workspaces-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:security+caa@improvado.io"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: improvado.io
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: improvado.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: developers.improvado.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 15:53:24 2026 GMT
  host: embedded.improvado.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Improvado Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Improvado, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Improvado
provider_slug: improvado
slug: improvado-domain-security
source_filename: improvado-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: improvado.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.improvado.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: embedded.improvado.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 15:53:24 2026 GMT\n  hsts: null\ndomains:\n- domain: improvado.io\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security+caa@improvado.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/improvado/security/improvado-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketing
- Marketing Intelligence
- Marketing Analytics
- Data Pipeline
- ETL
- Advertising Data
- Business Intelligence
- Data Integration
- AI Agents
- MCP
- Agent Readiness
---
