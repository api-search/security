---
anonymous_access: false
api_key_in: []
api_specs:
- filename: docsmint-com-admin-api-openapi.yml
  format: yaml
  label: docsmint-com Admin API
  slug: docsmint-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-admin-api-openapi.yml
- filename: docsmint-com-attachments-api-openapi.yml
  format: yaml
  label: docsmint-com Attachments API
  slug: docsmint-com-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-attachments-api-openapi.yml
- filename: docsmint-com-auth-api-openapi.yml
  format: yaml
  label: docsmint-com Auth API
  slug: docsmint-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-auth-api-openapi.yml
- filename: docsmint-com-categories-api-openapi.yml
  format: yaml
  label: docsmint-com Categories API
  slug: docsmint-com-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-categories-api-openapi.yml
- filename: docsmint-com-csrf-token-api-openapi.yml
  format: yaml
  label: docsmint-com Csrf Token API
  slug: docsmint-com-csrf-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-csrf-token-api-openapi.yml
- filename: docsmint-com-documents-api-openapi.yml
  format: yaml
  label: docsmint-com Documents API
  slug: docsmint-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-documents-api-openapi.yml
- filename: docsmint-com-folders-api-openapi.yml
  format: yaml
  label: docsmint-com Folders API
  slug: docsmint-com-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-folders-api-openapi.yml
- filename: docsmint-com-graph-api-openapi.yml
  format: yaml
  label: docsmint-com Graph API
  slug: docsmint-com-graph-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-graph-api-openapi.yml
- filename: docsmint-com-health-api-openapi.yml
  format: yaml
  label: docsmint-com Health API
  slug: docsmint-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-health-api-openapi.yml
- filename: docsmint-com-keys-api-openapi.yml
  format: yaml
  label: docsmint-com Keys API
  slug: docsmint-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-keys-api-openapi.yml
- filename: docsmint-com-plugins-api-openapi.yml
  format: yaml
  label: docsmint-com Plugins API
  slug: docsmint-com-plugins-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-plugins-api-openapi.yml
- filename: docsmint-com-search-api-openapi.yml
  format: yaml
  label: docsmint-com Search API
  slug: docsmint-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-search-api-openapi.yml
- filename: docsmint-com-share-api-openapi.yml
  format: yaml
  label: docsmint-com Share API
  slug: docsmint-com-share-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-share-api-openapi.yml
- filename: docsmint-com-tags-api-openapi.yml
  format: yaml
  label: docsmint-com Tags API
  slug: docsmint-com-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-tags-api-openapi.yml
- filename: docsmint-com-trash-api-openapi.yml
  format: yaml
  label: docsmint-com Trash API
  slug: docsmint-com-trash-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-trash-api-openapi.yml
- filename: docsmint-com-webhooks-api-openapi.yml
  format: yaml
  label: docsmint-com Webhooks API
  slug: docsmint-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Docsmint Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: docsmint-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: docsmint-com
provider_slug: docsmint-com
scheme_count: 2
schemes:
- bearerFormat: hiai_docs_*
  description: 'Send Authorization: Bearer <key> on every request. Create and revoke keys from DocsMint settings.'
  scheme: bearer
  type: http
- description: 'Workspace selection header. Send X-Docsmint-Workspace: <canonical-slug> to select workspace.'
  in: header
  name: X-Docsmint-Workspace
  type: apiKey
slug: docsmint-com-authentication
source_filename: docsmint-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://docsmint.com/docs/auth\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: \"hiai_docs_*\"\n    description: \"Send Authorization: Bearer <key> on every request. Create and revoke keys from DocsMint settings.\"\n  - type: apiKey\n    in: header\n    name: X-Docsmint-Workspace\n    description: \"Workspace selection header. Send X-Docsmint-Workspace: <canonical-slug> to select workspace.\"\n"
source_yaml_url: https://artifacts.apis.io/docsmint-com/authentication/docsmint-com-authentication.yml
summary_line: 2 schemes
tags:
- AI
- Document-Management
- Knowledge-Base
- SaaS
- Collaboration
---
