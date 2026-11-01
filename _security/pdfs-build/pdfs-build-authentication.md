---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pdfs-build-delegated-agents-api-openapi.yml
  format: yaml
  label: pdfs-build Delegated agents API
  slug: pdfs-build-delegated-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pdfs-build/openapi/pdfs-build-delegated-agents-api-openapi.yml
- filename: pdfs-build-embedded-editor-api-openapi.yml
  format: yaml
  label: pdfs-build Embedded editor API
  slug: pdfs-build-embedded-editor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pdfs-build/openapi/pdfs-build-embedded-editor-api-openapi.yml
- filename: pdfs-build-legacy-v1-api-openapi.yml
  format: yaml
  label: pdfs-build Legacy v1 API
  slug: pdfs-build-legacy-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pdfs-build/openapi/pdfs-build-legacy-v1-api-openapi.yml
- filename: pdfs-build-render-jobs-api-openapi.yml
  format: yaml
  label: pdfs-build Render jobs API
  slug: pdfs-build-render-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pdfs-build/openapi/pdfs-build-render-jobs-api-openapi.yml
- filename: pdfs-build-render-logs-api-openapi.yml
  format: yaml
  label: pdfs-build Render logs API
  slug: pdfs-build-render-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pdfs-build/openapi/pdfs-build-render-logs-api-openapi.yml
- filename: pdfs-build-rendering-api-openapi.yml
  format: yaml
  label: pdfs-build Rendering API
  slug: pdfs-build-rendering-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pdfs-build/openapi/pdfs-build-rendering-api-openapi.yml
- filename: pdfs-build-template-gallery-api-openapi.yml
  format: yaml
  label: pdfs-build Template gallery API
  slug: pdfs-build-template-gallery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pdfs-build/openapi/pdfs-build-template-gallery-api-openapi.yml
- filename: pdfs-build-templates-api-openapi.yml
  format: yaml
  label: pdfs-build Templates API
  slug: pdfs-build-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pdfs-build/openapi/pdfs-build-templates-api-openapi.yml
- filename: pdfs-build-webhooks-api-openapi.yml
  format: yaml
  label: pdfs-build Webhooks API
  slug: pdfs-build-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pdfs-build/openapi/pdfs-build-webhooks-api-openapi.yml
auth_types: []
description: Authentication for pdfs.build API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Pdfs Build Authentication
name_suffix: Authentication
oauth_flows: []
overview: pdfs-build declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: pdfs-build
provider_slug: pdfs-build
scheme_count: 1
schemes:
- evidence: 'curl -X POST https://api.pdfs.build/v2/organizations/YOUR_ORGANIZATION_ID/templates/invoice-primary/render \ -H "Authorization: Bearer prs_your_key_here" \ -H "Content-Type: application/json" \ -d ''{"data": {"company_name": "Acme Corp", "invoice_number": "INV-001"}}'''
  header: Authorization
  how_to_obtain: Grab your API key from Settings → API Keys in the pdfs.build dashboard.
  location: header
  name: Bearer
  type: http-bearer
slug: pdfs-build-authentication
source_filename: pdfs-build-authentication.yml
source_heading: Authentication Profile
source_url: https://pdfs.build/blog/getting-started/
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://pdfs.build/blog/getting-started/\nsources:\n- https://pdfs.build/blog/getting-started/\n- https://pdfs.build/blog/getting-started.md\ndescription: Authentication for pdfs.build API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'curl -X POST https://api.pdfs.build/v2/organizations/YOUR_ORGANIZATION_ID/templates/invoice-primary/render \\ -H \"Authorization: Bearer\n    prs_your_key_here\" \\ -H \"Content-Type: application/json\" \\ -d ''{\"data\": {\"company_name\": \"Acme Corp\", \"invoice_number\": \"INV-001\"}}'''\n  location: header\n  header: Authorization\n  how_to_obtain: Grab your API key from Settings → API Keys in the pdfs.build dashboard.\nnote: No other authentication schemes (e.g., OAuth2, apiKey query, etc.) are documented on the provided pages.\ndocs: https://pdfs.build/blog/getting-started/\n"
source_yaml_url: https://artifacts.apis.io/pdfs-build/authentication/pdfs-build-authentication.yml
summary_line: 1 scheme
tags:
- PDF
- API
- TemplateEngine
- Rendering
- SaaS
- DocumentGeneration
---
