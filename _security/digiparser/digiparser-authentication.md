---
anonymous_access: false
api_key_in: []
api_specs:
- filename: digiparser-document-processing-api-openapi.yml
  format: yaml
  label: DigiParser Document processing API
  slug: digiparser-document-processing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/digiparser/openapi/digiparser-document-processing-api-openapi.yml
- filename: digiparser-mcp-api-openapi.yml
  format: yaml
  label: DigiParser MCP API
  slug: digiparser-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/digiparser/openapi/digiparser-mcp-api-openapi.yml
- filename: digiparser-parsers-api-openapi.yml
  format: yaml
  label: DigiParser Parsers API
  slug: digiparser-parsers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/digiparser/openapi/digiparser-parsers-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Digiparser Authentication
name_suffix: Authentication
oauth_flows: []
overview: DigiParser declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: DigiParser
provider_slug: digiparser
scheme_count: 2
schemes:
- description: API key authentication for DigiParser endpoints.
  in: header
  name: X-API-Key
  type: apiKey
- description: MCP OAuth2 client credentials flow.
  flows:
    clientCredentials:
      scopes: {}
      tokenUrl: https://mcp.digiparser.com/.well-known/oauth-protected-resource/mcp
  type: oauth2
slug: digiparser-authentication
source_filename: digiparser-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: https://www.digiparser.com/openapi.json\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: API key authentication for DigiParser endpoints.\n  - type: oauth2\n    flows:\n      clientCredentials:\n        tokenUrl: https://mcp.digiparser.com/.well-known/oauth-protected-resource/mcp\n        scopes: {}\n    description: MCP OAuth2 client credentials flow.\n"
source_yaml_url: https://artifacts.apis.io/digiparser/authentication/digiparser-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Document-Processing
- API
- Automation
- Data-Extraction
- AI
---
