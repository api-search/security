---
anonymous_access: false
api_key_in: []
api_specs:
- filename: autokitteh-autokitteh-api-api-openapi.yml
  format: yaml
  label: AutoKitteh API
  slug: autokitteh-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autokitteh/openapi/autokitteh-autokitteh-api-api-openapi.yml
- filename: autokitteh-openapi-generated.yml
  format: yaml
  label: AutoKitteh API
  slug: autokitteh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autokitteh/openapi/_ae-authored/autokitteh-openapi-generated.yml
auth_types: []
description: Authentication methods for Linear integration as documented on AutoKitteh.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Autokitteh Authentication
name_suffix: Authentication
oauth_flows: []
overview: AutoKitteh declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: AutoKitteh
provider_slug: autokitteh
scheme_count: 3
schemes:
- evidence: Personal API keys provide a straightforward way to authenticate with the Linear API without going through the OAuth flow.
  how_to_obtain: See "How to get your API key in Linear" in the Linear documentation.
  name: Personal API Key
  type: apiKey
- evidence: OAuth 2.0 allows users to authorize your app to access their Linear workspace data.
  flows:
  - authorization_code
  how_to_obtain: Create a Linear OAuth App and configure the AutoKitteh server with LINEAR_CLIENT_ID and LINEAR_CLIENT_SECRET environment variables.
  name: Default OAuth 2.0 app
  type: oauth2
- evidence: OAuth 2.0 allows users to authorize your app to access their Linear workspace data.
  flows:
  - authorization_code
  how_to_obtain: Create a Linear OAuth App (following the Default OAuth guide) and provide the Client ID and Client Secret in the AutoKitteh connection configuration.
  name: Private OAuth 2.0 app
  type: oauth2
slug: autokitteh-authentication
source_filename: autokitteh-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.autokitteh.com/integrations/linear/api_key
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.autokitteh.com/integrations/linear/api_key\nsources:\n- https://docs.autokitteh.com/integrations/linear/api_key\n- https://docs.autokitteh.com/integrations/linear/default_oauth\n- https://docs.autokitteh.com/integrations/linear/private_oauth\n- https://docs.autokitteh.com/integrations/salesforce/private_oauth\ndescription: Authentication methods for Linear integration as documented on AutoKitteh.\nschemes:\n- type: apiKey\n  name: Personal API Key\n  evidence: Personal API keys provide a straightforward way to authenticate with the Linear API without going through the OAuth flow.\n  how_to_obtain: See \"How to get your API key in Linear\" in the Linear documentation.\n- type: oauth2\n  name: Default OAuth 2.0 app\n  evidence: OAuth 2.0 allows users to authorize your app to access their Linear workspace data.\n  flows:\n  - authorization_code\n  how_to_obtain: Create\
  \ a Linear OAuth App and configure the AutoKitteh server with LINEAR_CLIENT_ID and LINEAR_CLIENT_SECRET environment variables.\n- type: oauth2\n  name: Private OAuth 2.0 app\n  evidence: OAuth 2.0 allows users to authorize your app to access their Linear workspace data.\n  flows:\n  - authorization_code\n  how_to_obtain: Create a Linear OAuth App (following the Default OAuth guide) and provide the Client ID and Client Secret in the AutoKitteh connection\n    configuration.\ndocs: https://docs.autokitteh.com/integrations/linear/api_key\n"
source_yaml_url: https://artifacts.apis.io/autokitteh/authentication/autokitteh-authentication.yml
summary_line: 3 schemes
tags:
- Automation
- Orchestration
- Open Source
- Developer Tools
- Workflow Engine
---
