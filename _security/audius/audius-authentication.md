---
api_key_in: []
api_specs:
- filename: audius-openapi.yml
  format: yaml
  label: Audius REST API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Audius Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Audius secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Audius
provider_slug: audius
scheme_count: 3
schemes:
- description: 'OAuth 2.0 Authorization Code flow with PKCE for third-party applications.


    Allows apps to authenticate users and obtain access tokens scoped to read or read+write permissions on behalf of the user.


    **Scopes:**

    - `read` — Read-only access to the user''s public and private data.

    - `write` — Read and write access, allowing mutations on behalf of the user.


    **PKCE Required:**

    All authorization code re'
  flows:
  - authorizationUrl: /v1/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: /v1/oauth/token
  name: OAuth2
  sources:
  - openapi/audius-openapi.yml
  type: oauth2
- description: 'HTTP Basic Authentication with Ethereum private key for write operations.


    **Authentication**


    Use HTTP Basic Authentication where the password field contains your Ethereum private key:

    ```

    Authorization: Basic <base64(username:privatekey)>

    ```


    The username can be any value. The password must be your Ethereum private key in hex format (with or without 0x prefix).


    Example:

    ```

    Authorization: Basi'
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/audius-openapi.yml
  type: http
- bearerFormat: JWT
  description: The API bearer token or OAuth JWT token for the user.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/audius-openapi.yml
  type: http
slug: audius-authentication
source_filename: audius-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/audius-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /v1/oauth/authorize\n    tokenUrl: /v1/oauth/token\n    scopes: 2\n  description: |-\n    OAuth 2.0 Authorization Code flow with PKCE for third-party applications.\n\n    Allows apps to authenticate users and obtain access tokens scoped to read or read+write permissions on behalf of the user.\n\n    **Scopes:**\n    - `read` — Read-only access to the user's public and private data.\n    - `write` — Read and write access, allowing mutations on behalf of the user.\n\n    **PKCE Required:**\n    All authorization code re\n  sources:\n  - openapi/audius-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic Authentication with Ethereum private key for write operations.\n\n    **Authentication**\n\
  \n    Use HTTP Basic Authentication where the password field contains your Ethereum private key:\n    ```\n    Authorization: Basic <base64(username:privatekey)>\n    ```\n\n    The username can be any value. The password must be your Ethereum private key in hex format (with or without 0x prefix).\n\n    Example:\n    ```\n    Authorization: Basi\n  sources:\n  - openapi/audius-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: The API bearer token or OAuth JWT token for the user.\n  sources:\n  - openapi/audius-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/authentication/audius-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Music
- Streaming
- Decentralized
- Web3
- Open Source
- Blockchain
---
