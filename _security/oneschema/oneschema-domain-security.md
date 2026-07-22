---
api_specs:
- filename: oneschema-importer-embeds-openapi.yml
  format: yaml
  label: OneSchema Importer Embeds API
  slug: oneschema-importer-embeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-importer-embeds-openapi.yml
- filename: oneschema-templates-openapi.yml
  format: yaml
  label: OneSchema Templates API
  slug: oneschema-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-templates-openapi.yml
- filename: oneschema-sheets-openapi.yml
  format: yaml
  label: OneSchema Sheets API
  slug: oneschema-sheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-sheets-openapi.yml
- filename: oneschema-workspaces-openapi.yml
  format: yaml
  label: OneSchema Workspaces API
  slug: oneschema-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-workspaces-openapi.yml
- filename: oneschema-multi-filefeeds-openapi.yml
  format: yaml
  label: OneSchema Multi FileFeeds API
  slug: oneschema-multi-filefeeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-multi-filefeeds-openapi.yml
- filename: oneschema-filefeeds-openapi.yml
  format: yaml
  label: OneSchema FileFeeds API
  slug: oneschema-filefeeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-filefeeds-openapi.yml
- filename: oneschema-importer-webhooks-openapi.yml
  format: yaml
  label: OneSchema Importer Webhooks API
  slug: oneschema-importer-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-importer-webhooks-openapi.yml
- filename: oneschema-event-webhooks-openapi.yml
  format: yaml
  label: OneSchema Event Webhooks API
  slug: oneschema-event-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-event-webhooks-openapi.yml
- filename: oneschema-code-hooks-legacy-openapi.yml
  format: yaml
  label: OneSchema Code Hooks (Legacy) API
  slug: oneschema-code-hooks-legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-code-hooks-legacy-openapi.yml
- filename: oneschema-s3-accounts-openapi.yml
  format: yaml
  label: OneSchema S3 Accounts API
  slug: oneschema-s3-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-s3-accounts-openapi.yml
- filename: oneschema-sftp-accounts-openapi.yml
  format: yaml
  label: OneSchema SFTP Accounts API
  slug: oneschema-sftp-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-sftp-accounts-openapi.yml
- filename: oneschema-aws-secrets-manager-openapi.yml
  format: yaml
  label: OneSchema AWS Secrets Manager API
  slug: oneschema-aws-secrets-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-aws-secrets-manager-openapi.yml
- filename: oneschema-azure-key-vault-openapi.yml
  format: yaml
  label: OneSchema Azure Key Vault API
  slug: oneschema-azure-key-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-azure-key-vault-openapi.yml
- filename: oneschema-mcp-server-openapi.yml
  format: yaml
  label: OneSchema MCP Server API
  slug: oneschema-mcp-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-mcp-server-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oneschema.co
  spf: true
hosts:
- cert_expires: Sep  2 22:58:01 2026 GMT
  host: docs.oneschema.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: api.oneschema.co
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: api.eu.oneschema.co
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Oneschema Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oneschema, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oneschema
provider_slug: oneschema
slug: oneschema-domain-security
source_filename: oneschema-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.oneschema.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 22:58:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.oneschema.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: null\n- host: api.eu.oneschema.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: oneschema.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/security/oneschema-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Onboarding
- CSV Import
- Data Validation
- File Processing
- ETL
- Data Integration
- Embeddable UI
- Spreadsheets
- Developer Tools
- AI Data Transformation
---
