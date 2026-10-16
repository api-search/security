---
anonymous_access: false
api_key_in: []
api_specs:
- filename: carte-openapi-generated.yml
  format: yaml
  label: Carte API
  slug: carte-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carte/refs/heads/main/openapi/_ae-authored/carte-openapi-generated.yml
auth_types: []
description: Carta’s API uses OAuth 2.0 and supports the AUTHORIZATION_CODE and CLIENT_CREDENTIALS grant types.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Carte Authentication
name_suffix: Authentication
oauth_flows: []
overview: Carte declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Carte
provider_slug: carte
scheme_count: 1
schemes:
- evidence: Carta’s API uses the OAuth 2.0 open specification to authorize your access to our data, and supports AUTHORIZATION_CODE and CLIENT_CREDENTIALS grant types.
  how_to_obtain: You are provided a client_id and client_secret by Carta.
  name: Carta OAuth
  type: oauth2
slug: carte-authentication
source_filename: carte-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.carta.com/api-platform/guides/guides/authorization
source_yaml: "generated: '2026-10-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.carta.com/api-platform/guides/guides/authorization\nsources:\n- https://docs.carta.com/api-platform/guides/guides/authorization\n- https://docs.carta.com/api-platform/guides/guides/adding-new-oauth-scopes\n- https://docs.carta.com/api-platform/guides/guides/authorization/using-the-client-credentials-flow\n- https://docs.carta.com/api-platform/guides/guides/service-accounts\ndescription: Carta’s API uses OAuth 2.0 and supports the AUTHORIZATION_CODE and CLIENT_CREDENTIALS grant types.\nschemes:\n- type: oauth2\n  name: Carta OAuth\n  evidence: Carta’s API uses the OAuth 2.0 open specification to authorize your access to our data, and supports AUTHORIZATION_CODE and CLIENT_CREDENTIALS\n    grant types.\n  how_to_obtain: You are provided a client_id and client_secret by Carta.\ndocs: https://docs.carta.com/api-platform/guides/guides/authorization\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carte/refs/heads/main/authentication/carte-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Finance
- Equity
- FundManagement
- API
---
