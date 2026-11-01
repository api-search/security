---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for Mapped API using Personal Access Tokens
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mapped Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mapped declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Mapped
provider_slug: mapped-com
scheme_count: 1
schemes:
- evidence: All Mapped API calls will make use of a Personal Access Token
  header: Authorization
  how_to_obtain: generated on the Personal Access Token page of the Mapped Console
  location: header
  name: Personal Access Token
  type: apiKey
slug: mapped-com-authentication
source_filename: mapped-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.mapped.com/guides/platform/authentication-security.md
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (deepseek)\nsource: https://docs.mapped.com/guides/platform/authentication-security.md\nsources:\n- https://docs.mapped.com/guides/platform/authentication-security.md\n- https://docs.mapped.com/api/types/api-key.md\n- https://docs.mapped.com/api/types/api-key-input.md\n- https://docs.mapped.com/api/types/org-authentication-challenge.md\ndescription: Authentication for Mapped API using Personal Access Tokens\nschemes:\n- type: apiKey\n  name: Personal Access Token\n  evidence: All Mapped API calls will make use of a Personal Access Token\n  header: Authorization\n  location: header\n  how_to_obtain: generated on the Personal Access Token page of the Mapped Console\ndocs: https://docs.mapped.com/guides/platform/authentication-security.md\nnote: 'The documentation shows the token is passed as \"Authorization: token {TOKEN_VALUE}\" where \"token\" is the token type prefix'\n"
source_yaml_url: https://artifacts.apis.io/mapped-com/authentication/mapped-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Smart Buildings
- IoT
- GraphQL
- Data Integration
- Ontology
- Physical AI
- MCP
---
