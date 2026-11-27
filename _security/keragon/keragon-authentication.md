---
anonymous_access: false
api_key_in: []
api_specs:
- filename: keragon-openapi-generated.yml
  format: yaml
  label: Keragon API
  slug: keragon-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keragon/openapi/_ae-authored/keragon-openapi-generated.yml
auth_types: []
description: Keragon supports OAuth2 and API Key authentication schemes as described in its documentation.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Keragon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keragon declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Keragon
provider_slug: keragon
scheme_count: 2
schemes:
- authorize_url: https://provider.com/oauth2/authorize
  evidence: OAuth 2.0 is a widely used open standard for access delegation, commonly used for token-based authentication.
  flows:
  - authorizationCode
  - clientCredentials
  how_to_obtain: Users provide a client ID (and client secret) obtained from the vendor platform when configuring the connector.
  name: OAuth 2.0
  scopes:
  - read
  - write
  type: oauth2
- evidence: This method involves using a unique key to authenticate requests.
  header: Authorization
  how_to_obtain: Users enter the API key they received from the external service when creating the authentication in the Keragon workflow editor or CLI.
  location: header
  name: API Key
  type: apiKey
slug: keragon-authentication
source_filename: keragon-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.keragon.com/explanations/connector-authentication/index.md
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.keragon.com/explanations/connector-authentication/index.md\nsources:\n- https://docs.keragon.com/explanations/connector-authentication/index.md\n- https://docs.keragon.com/explanations/connector-authentication/authentication-schemes/index.md\n- https://docs.keragon.com/how-to-guides/connector-authentication/how-to-add-public-oauth2-app/index.md\n- https://docs.keragon.com/how-to-guides/connector-authentication/how-to-configure-api-key-auth/index.md\ndescription: Keragon supports OAuth2 and API Key authentication schemes as described in its documentation.\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: OAuth 2.0 is a widely used open standard for access delegation, commonly used for token-based authentication.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  authorize_url: https://provider.com/oauth2/authorize\n  scopes:\n  - read\n  - write\n  how_to_obtain:\
  \ Users provide a client ID (and client secret) obtained from the vendor platform when configuring the connector.\n- type: apiKey\n  name: API Key\n  evidence: This method involves using a unique key to authenticate requests.\n  location: header\n  header: Authorization\n  how_to_obtain: Users enter the API key they received from the external service when creating the authentication in the Keragon workflow editor\n    or CLI.\ndocs: https://docs.keragon.com/explanations/connector-authentication/index.md\n"
source_yaml_url: https://artifacts.apis.io/keragon/authentication/keragon-authentication.yml
summary_line: 2 schemes
tags:
- Healthcare
- Automation
- Artificial Intelligence
- Integration
- Compliance
- Company
---
