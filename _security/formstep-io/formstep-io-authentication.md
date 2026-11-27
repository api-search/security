---
anonymous_access: false
api_key_in: []
api_specs:
- filename: formstep-io-methods-api-openapi.yml
  format: yaml
  label: Formstep Methods API
  slug: formstep-io-methods-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formstep-io/openapi/formstep-io-methods-api-openapi.yml
auth_types: []
description: Formstep uses API tokens sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Formstep Authentication
name_suffix: Authentication
oauth_flows: []
overview: Formstep declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Formstep
provider_slug: formstep-io
scheme_count: 1
schemes:
- evidence: 'Send it as a bearer token:'
  header: Authorization
  how_to_obtain: Create a token in the **OAuth and API Keys** page under the API Keys card.
  location: header
  name: API token
  type: http-bearer
slug: formstep-io-authentication
source_filename: formstep-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.formstep.io/sharing-publishing/authentication-gate.md
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.formstep.io/sharing-publishing/authentication-gate.md\nsources:\n- https://docs.formstep.io/sharing-publishing/authentication-gate.md\n- https://docs.formstep.io/requests/callbacks.md\n- https://docs.formstep.io/developers/api-tokens.md\n- https://docs.formstep.io/getting-started/introduction.md\ndescription: Formstep uses API tokens sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: API token\n  evidence: 'Send it as a bearer token:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a token in the **OAuth and API Keys** page under the API Keys card.\nnote: No other authentication methods (e.g., OAuth2, apiKey) are documented on the provided pages.\ndocs: https://docs.formstep.io/sharing-publishing/authentication-gate.md\n"
source_yaml_url: https://artifacts.apis.io/formstep-io/authentication/formstep-io-authentication.yml
summary_line: 1 scheme
tags:
- Forms
- Automation
- Data Collection
- Workflow Integration
- Software-as-a-Service
---
