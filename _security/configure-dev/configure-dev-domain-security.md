---
api_specs:
- filename: configure-dev-auth-api-openapi.yml
  format: yaml
  label: Configure Auth API
  slug: configure-dev-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configure-dev/openapi/configure-dev-auth-api-openapi.yml
- filename: configure-dev-connectors-api-openapi.yml
  format: yaml
  label: Configure Connectors API
  slug: configure-dev-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configure-dev/openapi/configure-dev-connectors-api-openapi.yml
- filename: configure-dev-files-api-openapi.yml
  format: yaml
  label: Configure Files API
  slug: configure-dev-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configure-dev/openapi/configure-dev-files-api-openapi.yml
- filename: configure-dev-import-api-openapi.yml
  format: yaml
  label: Configure Import API
  slug: configure-dev-import-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configure-dev/openapi/configure-dev-import-api-openapi.yml
- filename: configure-dev-profile-api-openapi.yml
  format: yaml
  label: Configure Profile API
  slug: configure-dev-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configure-dev/openapi/configure-dev-profile-api-openapi.yml
- filename: configure-dev-web-api-openapi.yml
  format: yaml
  label: Configure Web API
  slug: configure-dev-web-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configure-dev/openapi/configure-dev-web-api-openapi.yml
- filename: configure-dev-webhooks-api-openapi.yml
  format: yaml
  label: Configure Webhooks API
  slug: configure-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configure-dev/openapi/configure-dev-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: configure.dev
  spf: true
hosts:
- cert_expires: Jan 16 23:30:51 2027 GMT
  host: configure.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Configure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Configure, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Configure
provider_slug: configure-dev
slug: configure-dev-domain-security
source_filename: configure-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: configure.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:30:51 2027 GMT\n  hsts: false\ndomains:\n- domain: configure.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/configure-dev/security/configure-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Memory
- Personalization
- User Context
- MCP
---
