---
anonymous_access: false
api_key_in: []
api_specs:
- filename: carta-fa464-openapi-generated.yml
  format: yaml
  label: Carta Fa464 API
  slug: carta-fa464-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carta-fa464/refs/heads/main/openapi/_ae-authored/carta-fa464-openapi-generated.yml
auth_types: []
description: Authentication schemes for Carta API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Carta Fa464 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Carta Fa464 declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Carta Fa464
provider_slug: carta-fa464
scheme_count: 1
schemes:
- evidence: Carta’s API uses the OAuth 2.0 open specification to authorize your access to our data, and supports AUTHORIZATION_CODE and CLIENT_CREDENTIALS grant types.
  flows:
  - authorization_code
  - client_credentials
  how_to_obtain: client_id and client_secret issued by Carta
  name: Carta OAuth2
  token_url: https://login.app.carta.com/o/access_token/
  type: oauth2
slug: carta-fa464-authentication
source_filename: carta-fa464-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.carta.com/api-platform/guides/guides/authorization
source_yaml: "generated: '2026-10-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.carta.com/api-platform/guides/guides/authorization\nsources:\n- https://docs.carta.com/api-platform/guides/guides/authorization\n- https://docs.carta.com/api-platform/guides/guides/adding-new-oauth-scopes\n- https://docs.carta.com/api-platform/guides/guides/authorization/using-the-client-credentials-flow\n- https://docs.carta.com/api-platform/guides/guides/service-accounts\ndescription: Authentication schemes for Carta API\nschemes:\n- type: oauth2\n  name: Carta OAuth2\n  evidence: Carta’s API uses the OAuth 2.0 open specification to authorize your access to our data, and supports AUTHORIZATION_CODE and CLIENT_CREDENTIALS\n    grant types.\n  flows:\n  - authorization_code\n  - client_credentials\n  token_url: https://login.app.carta.com/o/access_token/\n  how_to_obtain: client_id and client_secret issued by Carta\ndocs: https://docs.carta.com/api-platform/guides/guides/authorization\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carta-fa464/refs/heads/main/authentication/carta-fa464-authentication.yml
summary_line: 1 scheme
tags:
- Equity Management
- Fund Administration
- Legal Compliance
- Cap Table
- Valuations
- Private Capital
- CRM Integration
- AI Automation
---
