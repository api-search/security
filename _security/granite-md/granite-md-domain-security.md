---
api_specs:
- filename: granite-md-auth-api-openapi.yml
  format: yaml
  label: Granite Auth API
  slug: granite-md-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-auth-api-openapi.yml
- filename: granite-md-billing-api-openapi.yml
  format: yaml
  label: Granite Billing API
  slug: granite-md-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-billing-api-openapi.yml
- filename: granite-md-comments-api-openapi.yml
  format: yaml
  label: Granite Comments API
  slug: granite-md-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-comments-api-openapi.yml
- filename: granite-md-drive-api-openapi.yml
  format: yaml
  label: Granite Drive API
  slug: granite-md-drive-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-drive-api-openapi.yml
- filename: granite-md-folders-api-openapi.yml
  format: yaml
  label: Granite Folders API
  slug: granite-md-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-folders-api-openapi.yml
- filename: granite-md-knowledge-base-api-openapi.yml
  format: yaml
  label: Granite knowledge base API
  slug: granite-md-knowledge-base-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-knowledge-base-api-openapi.yml
- filename: granite-md-me-api-openapi.yml
  format: yaml
  label: Granite Me API
  slug: granite-md-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-me-api-openapi.yml
- filename: granite-md-meta-api-openapi.yml
  format: yaml
  label: Granite Meta API
  slug: granite-md-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-meta-api-openapi.yml
- filename: granite-md-note-shares-api-openapi.yml
  format: yaml
  label: Granite Note Shares API
  slug: granite-md-note-shares-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-note-shares-api-openapi.yml
- filename: granite-md-notes-api-openapi.yml
  format: yaml
  label: Granite Notes API
  slug: granite-md-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-notes-api-openapi.yml
- filename: granite-md-oauth-api-openapi.yml
  format: yaml
  label: Granite OAuth API
  slug: granite-md-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-oauth-api-openapi.yml
- filename: granite-md-publish-api-openapi.yml
  format: yaml
  label: Granite Publish API
  slug: granite-md-publish-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-publish-api-openapi.yml
- filename: granite-md-search-api-openapi.yml
  format: yaml
  label: Granite Search API
  slug: granite-md-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-search-api-openapi.yml
- filename: granite-md-shopify-api-openapi.yml
  format: yaml
  label: Granite Shopify API
  slug: granite-md-shopify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-shopify-api-openapi.yml
- filename: granite-md-sync-api-openapi.yml
  format: yaml
  label: Granite Sync API
  slug: granite-md-sync-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-sync-api-openapi.yml
- filename: granite-md-templates-api-openapi.yml
  format: yaml
  label: Granite Templates API
  slug: granite-md-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-templates-api-openapi.yml
- filename: granite-md-vaults-api-openapi.yml
  format: yaml
  label: Granite Vaults API
  slug: granite-md-vaults-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-vaults-api-openapi.yml
- filename: granite-md-webhooks-api-openapi.yml
  format: yaml
  label: Granite Webhooks API
  slug: granite-md-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-webhooks-api-openapi.yml
- filename: granite-md-workspaces-api-openapi.yml
  format: yaml
  label: Granite Workspaces API
  slug: granite-md-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: granite.md
  spf: true
hosts:
- cert_expires: Jan  3 12:45:21 2027 GMT
  host: granite.md
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Granite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Granite, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Granite
provider_slug: granite-md
slug: granite-md-domain-security
source_filename: granite-md-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: granite.md\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 12:45:21 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: granite.md\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/granite-md/security/granite-md-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Knowledge Base
- Artificial Intelligence
- Collaboration
- Security
- Encryption
---
