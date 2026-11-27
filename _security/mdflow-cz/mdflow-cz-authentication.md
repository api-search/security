---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mdflow-cz-documents-api-openapi.yml
  format: yaml
  label: MDflow Documents API
  slug: mdflow-cz-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mdflow-cz/openapi/mdflow-cz-documents-api-openapi.yml
- filename: mdflow-cz-folders-api-openapi.yml
  format: yaml
  label: MDflow Folders API
  slug: mdflow-cz-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mdflow-cz/openapi/mdflow-cz-folders-api-openapi.yml
- filename: mdflow-cz-team-documents-api-openapi.yml
  format: yaml
  label: MDflow Team documents API
  slug: mdflow-cz-team-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mdflow-cz/openapi/mdflow-cz-team-documents-api-openapi.yml
- filename: mdflow-cz-team-folders-api-openapi.yml
  format: yaml
  label: MDflow Team folders API
  slug: mdflow-cz-team-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mdflow-cz/openapi/mdflow-cz-team-folders-api-openapi.yml
- filename: mdflow-cz-team-workspaces-api-openapi.yml
  format: yaml
  label: MDflow Team workspaces API
  slug: mdflow-cz-team-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mdflow-cz/openapi/mdflow-cz-team-workspaces-api-openapi.yml
- filename: mdflow-cz-workspaces-api-openapi.yml
  format: yaml
  label: MDflow Workspaces API
  slug: mdflow-cz-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mdflow-cz/openapi/mdflow-cz-workspaces-api-openapi.yml
auth_types: []
description: 'MDflow authenticates clients using a Personal Access Token (a token that starts with "mdf_") sent in an Authorization: Bearer header.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: MDflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: MDflow declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MDflow
provider_slug: mdflow-cz
scheme_count: 1
schemes:
- evidence: 'TL;DR — Create a Personal Access Token in MDflow Settings (starts with mdf_ ). For the hosted server, point your client at https://mdflow.cz/api/mcp with an Authorization: Bearer header'
  header: Authorization
  how_to_obtain: Create a Personal Access Token in MDflow Settings; the token starts with "mdf_".
  name: Personal Access Token
  type: http-bearer
slug: mdflow-cz-authentication
source_filename: mdflow-cz-authentication.yml
source_heading: Authentication Profile
source_url: https://mdflow.cz/blog/agent-authorization-scoped-tokens
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mdflow.cz/blog/agent-authorization-scoped-tokens\nsources:\n- https://mdflow.cz/blog/agent-authorization-scoped-tokens\n- https://mdflow.cz/blog/agent-authentication\n- https://mdflow.cz/blog/mdflow-mcp-setup-cursor-claude-desktop-codex\ndescription: 'MDflow authenticates clients using a Personal Access Token (a token that starts with \"mdf_\") sent in an Authorization: Bearer header.'\nschemes:\n- type: http-bearer\n  name: Personal Access Token\n  evidence: 'TL;DR — Create a Personal Access Token in MDflow Settings (starts with mdf_ ). For the hosted server, point your client at https://mdflow.cz/api/mcp\n    with an Authorization: Bearer header'\n  header: Authorization\n  how_to_obtain: Create a Personal Access Token in MDflow Settings; the token starts with \"mdf_\".\nnote: No other authentication schemes (apiKey, oauth2, http-basic, etc.) are described on the provided\
  \ pages.\ndocs: https://mdflow.cz/blog/agent-authorization-scoped-tokens\n"
source_yaml_url: https://artifacts.apis.io/mdflow-cz/authentication/mdflow-cz-authentication.yml
summary_line: 1 scheme
tags:
- Markdown editor
- Knowledge Base
- AI Agents
- Web clipper
---
