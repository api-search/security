---
api_specs:
- filename: mcphost-dev-assets-api-openapi.yml
  format: yaml
  label: mcphost Assets API
  slug: mcphost-dev-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcphost-dev/openapi/mcphost-dev-assets-api-openapi.yml
- filename: mcphost-dev-billing-api-openapi.yml
  format: yaml
  label: mcphost Billing API
  slug: mcphost-dev-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcphost-dev/openapi/mcphost-dev-billing-api-openapi.yml
- filename: mcphost-dev-claim-api-openapi.yml
  format: yaml
  label: mcphost Claim API
  slug: mcphost-dev-claim-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcphost-dev/openapi/mcphost-dev-claim-api-openapi.yml
- filename: mcphost-dev-help-api-openapi.yml
  format: yaml
  label: mcphost Help API
  slug: mcphost-dev-help-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcphost-dev/openapi/mcphost-dev-help-api-openapi.yml
- filename: mcphost-dev-oauth-api-openapi.yml
  format: yaml
  label: mcphost OAuth API
  slug: mcphost-dev-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcphost-dev/openapi/mcphost-dev-oauth-api-openapi.yml
- filename: mcphost-dev-onboarding-api-openapi.yml
  format: yaml
  label: mcphost Onboarding API
  slug: mcphost-dev-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcphost-dev/openapi/mcphost-dev-onboarding-api-openapi.yml
- filename: mcphost-dev-public-tool-api-openapi.yml
  format: yaml
  label: mcphost Public Tool API
  slug: mcphost-dev-public-tool-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcphost-dev/openapi/mcphost-dev-public-tool-api-openapi.yml
- filename: mcphost-dev-status-api-openapi.yml
  format: yaml
  label: mcphost Status API
  slug: mcphost-dev-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcphost-dev/openapi/mcphost-dev-status-api-openapi.yml
- filename: mcphost-dev-webhooks-api-openapi.yml
  format: yaml
  label: mcphost Webhooks API
  slug: mcphost-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcphost-dev/openapi/mcphost-dev-webhooks-api-openapi.yml
- filename: mcphost-dev-well-known-api-openapi.yml
  format: yaml
  label: mcphost Well Known API
  slug: mcphost-dev-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcphost-dev/openapi/mcphost-dev-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mcphost.dev
  spf: true
hosts:
- cert_expires: Feb  3 03:39:57 2027 GMT
  host: mcphost.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: mcphost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mcphost, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: mcphost
provider_slug: mcphost-dev
slug: mcphost-dev-domain-security
source_filename: mcphost-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcphost.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 03:39:57 2027 GMT\n  hsts: false\ndomains:\n- domain: mcphost.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mcphost-dev/security/mcphost-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Hosting
- MCP
- Tools
- Platform
---
