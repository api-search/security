---
api_key_in: []
api_specs:
- filename: audius-challenges-api-openapi.yml
  format: yaml
  label: Audius challenges API
  slug: audius-challenges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-challenges-api-openapi.yml
- filename: audius-cid-data-api-openapi.yml
  format: yaml
  label: Audius cid_data API
  slug: audius-cid-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-cid-data-api-openapi.yml
- filename: audius-coins-api-openapi.yml
  format: yaml
  label: Audius coins API
  slug: audius-coins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-coins-api-openapi.yml
- filename: audius-comments-api-openapi.yml
  format: yaml
  label: Audius comments API
  slug: audius-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-comments-api-openapi.yml
- filename: audius-dashboard-wallet-users-api-openapi.yml
  format: yaml
  label: Audius dashboard_wallet_users API
  slug: audius-dashboard-wallet-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-dashboard-wallet-users-api-openapi.yml
- filename: audius-developer-apps-api-openapi.yml
  format: yaml
  label: Audius developer_apps API
  slug: audius-developer-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-developer-apps-api-openapi.yml
- filename: audius-events-api-openapi.yml
  format: yaml
  label: Audius events API
  slug: audius-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-events-api-openapi.yml
- filename: audius-explore-api-openapi.yml
  format: yaml
  label: Audius explore API
  slug: audius-explore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-explore-api-openapi.yml
- filename: audius-notifications-api-openapi.yml
  format: yaml
  label: Audius notifications API
  slug: audius-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-notifications-api-openapi.yml
- filename: audius-playlists-api-openapi.yml
  format: yaml
  label: Audius playlists API
  slug: audius-playlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-playlists-api-openapi.yml
- filename: audius-prizes-api-openapi.yml
  format: yaml
  label: Audius prizes API
  slug: audius-prizes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-prizes-api-openapi.yml
- filename: audius-reactions-api-openapi.yml
  format: yaml
  label: Audius reactions API
  slug: audius-reactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-reactions-api-openapi.yml
- filename: audius-resolve-api-openapi.yml
  format: yaml
  label: Audius resolve API
  slug: audius-resolve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-resolve-api-openapi.yml
- filename: audius-rewards-api-openapi.yml
  format: yaml
  label: Audius rewards API
  slug: audius-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-rewards-api-openapi.yml
- filename: audius-search-api-openapi.yml
  format: yaml
  label: Audius search API
  slug: audius-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-search-api-openapi.yml
- filename: audius-tips-api-openapi.yml
  format: yaml
  label: Audius tips API
  slug: audius-tips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-tips-api-openapi.yml
- filename: audius-tracks-api-openapi.yml
  format: yaml
  label: Audius tracks API
  slug: audius-tracks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-tracks-api-openapi.yml
- filename: audius-transactions-api-openapi.yml
  format: yaml
  label: Audius transactions API
  slug: audius-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-transactions-api-openapi.yml
- filename: audius-users-api-openapi.yml
  format: yaml
  label: Audius users API
  slug: audius-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-users-api-openapi.yml
- filename: audius-wallet-api-openapi.yml
  format: yaml
  label: Audius wallet API
  slug: audius-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-wallet-api-openapi.yml
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
