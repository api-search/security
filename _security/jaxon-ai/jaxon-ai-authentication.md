---
anonymous_access: false
api_key_in: []
api_specs:
- filename: jaxon-ai-check-api-openapi.yml
  format: yaml
  label: Jaxon Check API
  slug: jaxon-ai-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jaxon-ai/openapi/jaxon-ai-check-api-openapi.yml
- filename: jaxon-ai-extraction-api-openapi.yml
  format: yaml
  label: Jaxon Extraction API
  slug: jaxon-ai-extraction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jaxon-ai/openapi/jaxon-ai-extraction-api-openapi.yml
- filename: jaxon-ai-operations-api-openapi.yml
  format: yaml
  label: Jaxon Operations API
  slug: jaxon-ai-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jaxon-ai/openapi/jaxon-ai-operations-api-openapi.yml
- filename: jaxon-ai-ruleset-api-openapi.yml
  format: yaml
  label: Jaxon Ruleset API
  slug: jaxon-ai-ruleset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jaxon-ai/openapi/jaxon-ai-ruleset-api-openapi.yml
- filename: jaxon-ai-teams-api-openapi.yml
  format: yaml
  label: Jaxon Teams API
  slug: jaxon-ai-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jaxon-ai/openapi/jaxon-ai-teams-api-openapi.yml
- filename: jaxon-ai-units-api-openapi.yml
  format: yaml
  label: Jaxon Units API
  slug: jaxon-ai-units-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jaxon-ai/openapi/jaxon-ai-units-api-openapi.yml
auth_types: []
description: Authentication methods for Jaxon Platform API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Jaxon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jaxon declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Jaxon
provider_slug: jaxon-ai
scheme_count: 2
schemes:
- evidence: The Jaxon web application authenticates users via OAuth 2.0 Authorization Code with PKCE .
  how_to_obtain: The UI performs the PKCE flow automatically when a user logs in through the browser; no manual configuration is required.
  name: Jaxon UI OAuth
  type: oauth2
- evidence: The API token can be used directly as a Bearer token in API requests along with the X-Jaxon-Active-Group header.
  header: Authorization
  how_to_obtain: A platform administrator creates a service account in Authentik, assigns it to groups, and creates an API token via the Authentik admin portal (Directory > Tokens and App passwords).
  location: header
  name: API token
  type: http-bearer
slug: jaxon-ai-authentication
source_filename: jaxon-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.jaxon.ai/reference/authentication/
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.jaxon.ai/reference/authentication/\nsources:\n- https://docs.jaxon.ai/reference/authentication/\n- https://docs.agents.jaxon.ai/quickstart/claude-ai.html\n- https://docs.agents.jaxon.ai/quickstart/chatgpt.html\n- https://docs.agents.jaxon.ai/quickstart/claude-code.html\ndescription: Authentication methods for Jaxon Platform API\nschemes:\n- type: oauth2\n  name: Jaxon UI OAuth\n  evidence: The Jaxon web application authenticates users via OAuth 2.0 Authorization Code with PKCE .\n  how_to_obtain: The UI performs the PKCE flow automatically when a user logs in through the browser; no manual configuration is required.\n- type: http-bearer\n  name: API token\n  evidence: The API token can be used directly as a Bearer token in API requests along with the X-Jaxon-Active-Group header.\n  location: header\n  header: Authorization\n  how_to_obtain: A platform administrator\
  \ creates a service account in Authentik, assigns it to groups, and creates an API token via the Authentik\n    admin portal (Directory > Tokens and App passwords).\ndocs: https://docs.jaxon.ai/reference/authentication/\n"
source_yaml_url: https://artifacts.apis.io/jaxon-ai/authentication/jaxon-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Compliance
- Defense
- Finance
- Insurance
---
