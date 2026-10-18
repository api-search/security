---
anonymous_access: false
api_key_in: []
api_specs:
- filename: 0codekit-ai-api-openapi.yml
  format: yaml
  label: relyon AI API
  slug: 0codekit-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0codekit/refs/heads/main/openapi/0codekit-ai-api-openapi.yml
- filename: 0codekit-docs-api-openapi.yml
  format: yaml
  label: relyon Docs API
  slug: 0codekit-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0codekit/refs/heads/main/openapi/0codekit-docs-api-openapi.yml
- filename: 0codekit-image-api-openapi.yml
  format: yaml
  label: relyon Image API
  slug: 0codekit-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0codekit/refs/heads/main/openapi/0codekit-image-api-openapi.yml
- filename: 0codekit-mcp-api-openapi.yml
  format: yaml
  label: relyon MCP API
  slug: 0codekit-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0codekit/refs/heads/main/openapi/0codekit-mcp-api-openapi.yml
- filename: 0codekit-pdf-api-openapi.yml
  format: yaml
  label: relyon PDF API
  slug: 0codekit-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0codekit/refs/heads/main/openapi/0codekit-pdf-api-openapi.yml
auth_types: []
description: Authentication schemes for relyon
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: 0Codekit Authentication
name_suffix: Authentication
oauth_flows: []
overview: relyon declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: relyon
provider_slug: 0codekit
scheme_count: 1
schemes:
- evidence: Header Parameters ipaas string
  header: ipaas
  location: header
  name: ipaas
  type: apiKey
slug: 0codekit-authentication
source_filename: 0codekit-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.0codekit.com/main/api-keys/
source_yaml: "generated: '2026-10-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.0codekit.com/main/api-keys/\nsources:\n- https://docs.0codekit.com/main/api-keys/\n- https://docs.0codekit.com/api/1-saas-auth-post/\n- https://docs.0codekit.com/category/getting-started/\n- https://docs.0codekit.com/main/getting-started/make/\ndescription: Authentication schemes for relyon\nschemes:\n- type: apiKey\n  name: ipaas\n  evidence: Header Parameters ipaas string\n  location: header\n  header: ipaas\ndocs: https://docs.0codekit.com/main/api-keys/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/0codekit/refs/heads/main/authentication/0codekit-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Low-Code
- No-Code
- PDF Tools
- AI Integration
---
