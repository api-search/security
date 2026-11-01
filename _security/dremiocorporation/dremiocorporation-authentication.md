---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dremiocorporation-openapi-generated.yml
  format: yaml
  label: Dremiocorporation API
  slug: dremiocorporation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dremiocorporation/openapi/_ae-authored/dremiocorporation-openapi-generated.yml
auth_types: []
description: Authentication methods for Dremio Cloud and Dremio Enterprise
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Dremiocorporation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dremiocorporation declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Dremiocorporation
provider_slug: dremiocorporation
scheme_count: 2
schemes:
- evidence: The client ID and client secret are used to obtain a short-lived access token for a service user that provides secure, time-limited access to resources.
  flows:
  - client_credentials
  how_to_obtain: Create a service user in the Dremio console to get a client ID and client secret, then POST to the token URL with grant_type=client_credentials.
  name: OAuth Client Credentials
  scopes:
  - dremio.all
  token_url: https://login.dremio.cloud/oauth/token
  type: oauth2
- evidence: Applications can exchange JSON Web Tokens (JWTs) from external token providers for Dremio OAuth access tokens.
  flows:
  - urn:ietf:params:oauth:grant-type:token-exchange
  how_to_obtain: Obtain a JWT from an external OIDC provider, then POST to the token URL with subject_token, subject_token_type, grant_type=urn:ietf:params:oauth:grant-type:token-exchange, and scope.
  name: External JWT Exchange
  scopes:
  - dremio.all
  token_url: https://login.dremio.cloud/oauth/token
  type: oauth2
slug: dremiocorporation-authentication
source_filename: dremiocorporation-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.dremio.com/dremio-cloud/security/authentication/
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.dremio.com/dremio-cloud/security/authentication/\nsources:\n- https://docs.dremio.com/dremio-cloud/security/authentication/\n- https://docs.dremio.com/dremio-cloud/api/oauth-token/\n- https://docs.dremio.com/current/security/authentication/\n- https://docs.dremio.com/current/security/authentication/\ndescription: Authentication methods for Dremio Cloud and Dremio Enterprise\nschemes:\n- type: oauth2\n  name: OAuth Client Credentials\n  evidence: The client ID and client secret are used to obtain a short-lived access token for a service user that provides secure, time-limited\n    access to resources.\n  flows:\n  - client_credentials\n  token_url: https://login.dremio.cloud/oauth/token\n  scopes:\n  - dremio.all\n  how_to_obtain: Create a service user in the Dremio console to get a client ID and client secret, then POST to the token URL with grant_type=client_credentials.\n\
  - type: oauth2\n  name: External JWT Exchange\n  evidence: Applications can exchange JSON Web Tokens (JWTs) from external token providers for Dremio OAuth access tokens.\n  flows:\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  token_url: https://login.dremio.cloud/oauth/token\n  scopes:\n  - dremio.all\n  how_to_obtain: Obtain a JWT from an external OIDC provider, then POST to the token URL with subject_token, subject_token_type, grant_type=urn:ietf:params:oauth:grant-type:token-exchange,\n    and scope.\ndocs: https://docs.dremio.com/dremio-cloud/security/authentication/\n"
source_yaml_url: https://artifacts.apis.io/dremiocorporation/authentication/dremiocorporation-authentication.yml
summary_line: 2 schemes
tags:
- Data
- Lakehouse
- Analytics
- AI
- SAP
---
