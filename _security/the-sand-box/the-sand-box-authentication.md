---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: The Sand Box Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Sandbox declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: The Sandbox
provider_slug: the-sand-box
scheme_count: 2
schemes:
- authorization_endpoint: null
  credentials:
    client_id: issued by The Sandbox on approval of a developer access request
    client_secret: issued by The Sandbox on approval of a developer access request
    redirect_uri: registered per application; deep-link schemes are supported for desktop builds
  documented: true
  endpoint_note: The concrete authorize/token URLs are not stated on any page that loaded. They live behind the 503 authentication page. Not guessed.
  flow: authorization_code
  flow_evidence: The Unity SDK reference documents RequestAuthorization() ("starts the browser authentication flow") followed by RequestToken(string code) ("Requests a token using the provided code") - an authorization-code exchange. The published OAuthSettings object carries clientId, clientSecret and redirectUri, and the shipped Avatar Demo uses a custom-scheme redirect ("avatardemo://auth").
  id: oauth2
  refresh_tokens:
    note: The API Reference security guidance says "Handle expiration and use refresh tokens"; the Unity SDK FAQ states the SDK "manages token refreshing internally".
    supported: true
  scopes:
    documented: false
    note: Scopes exist in the model - the SDK FAQ says OAuthSettings takes "client ID, scopes, etc." and the API Reference tells integrators to "Scope tokens properly to limit access" - but NO scope reference page is published anywhere we can reach, and the page that would carry it (/api/authentication.html) is 503. No scopes/ artifact is emitted rather than inventing values.
  token_endpoint: null
  type: oauth2
- documented: true
  evidence: API Reference status-code table, 401 `unauthenticated` - "Invalid or missing bearer token".
  id: bearer
  in: header
  note: The bearer token is the OAuth access token from the flow above; it is not a separately issued static API key.
  scheme: bearer
  type: http
slug: the-sand-box-authentication
source_filename: the-sand-box-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: >-\n  https://developers.sandbox.game/api/ (API Reference: Additional Security Considerations, Status\n  Codes) + https://developers.sandbox.game/what-is/ + https://developers.sandbox.game/getting-started/\n  + https://developers.sandbox.game/unity/reference/ + https://developers.sandbox.game/unity/examples/\n  + https://developers.sandbox.game/unity/faq/\nsummary: >-\n  The Sandbox Developers API is protected by an OAuth-based identity system. A developer is issued a\n  client id and client secret out of band (by request and approval), runs a browser authorization\n  flow against the user's Sandbox account, exchanges the resulting code for a token, and calls the\n  REST API with a bearer token. The API returns 401 `unauthenticated` for an invalid or missing\n  bearer token and 403 `unauthorized` for insufficient permissions, which confirms both a bearer\n  scheme and a permission/scope model on the wire.\nderived_from_spec:\
  \ false\nspec_note: >-\n  DERIVED FROM DOCS ONLY. No OpenAPI document could be read for this provider - see\n  conformance/the-sand-box-conformance.yml and lifecycle/the-sand-box-lifecycle.yml for the probe\n  record. The Handling Authentication page (https://developers.sandbox.game/api/authentication.html)\n  and the Swagger playground (https://developers.sandbox.game/api/docs/) both returned HTTP 503 from\n  nginx on 2026-08-30, so the authoritative auth reference could not be captured. Everything below\n  comes from pages that DID load; nothing here is inferred beyond what those pages state.\nschemes:\n- id: oauth2\n  type: oauth2\n  documented: true\n  flow: authorization_code\n  flow_evidence: >-\n    The Unity SDK reference documents RequestAuthorization() (\"starts the browser authentication\n    flow\") followed by RequestToken(string code) (\"Requests a token using the provided code\") - an\n    authorization-code exchange. The published OAuthSettings object carries clientId,\
  \ clientSecret\n    and redirectUri, and the shipped Avatar Demo uses a custom-scheme redirect (\"avatardemo://auth\").\n  credentials:\n    client_id: issued by The Sandbox on approval of a developer access request\n    client_secret: issued by The Sandbox on approval of a developer access request\n    redirect_uri: registered per application; deep-link schemes are supported for desktop builds\n  scopes:\n    documented: false\n    note: >-\n      Scopes exist in the model - the SDK FAQ says OAuthSettings takes \"client ID, scopes, etc.\" and\n      the API Reference tells integrators to \"Scope tokens properly to limit access\" - but NO scope\n      reference page is published anywhere we can reach, and the page that would carry it\n      (/api/authentication.html) is 503. No scopes/ artifact is emitted rather than inventing values.\n  refresh_tokens:\n    supported: true\n    note: >-\n      The API Reference security guidance says \"Handle expiration and use refresh tokens\"; the Unity\n\
  \      SDK FAQ states the SDK \"manages token refreshing internally\".\n  token_endpoint: null\n  authorization_endpoint: null\n  endpoint_note: >-\n    The concrete authorize/token URLs are not stated on any page that loaded. They live behind the\n    503 authentication page. Not guessed.\n- id: bearer\n  type: http\n  scheme: bearer\n  documented: true\n  in: header\n  evidence: >-\n    API Reference status-code table, 401 `unauthenticated` - \"Invalid or missing bearer token\".\n  note: >-\n    The bearer token is the OAuth access token from the flow above; it is not a separately issued\n    static API key.\nauthorization:\n  model: permission-scoped bearer token\n  failure_codes:\n  - status: 401\n    code: unauthenticated\n    meaning: Invalid or missing bearer token\n  - status: 403\n    code: unauthorized\n    meaning: Insufficient permissions\naccess_model:\n  onboarding: request-and-approve\n  steps:\n  - Request access to the Developer API from the Developers HUB.\n  - Wait for\
  \ The Sandbox team to review and approve the request.\n  - Receive API credentials (OAuth client id and client secret) from The Sandbox.\n  source: https://developers.sandbox.game/getting-started/\n  note: >-\n    There is no self-serve key issuance. A developer account, a Sandbox user account and a GitHub\n    account are the stated prerequisites (the GitHub account is needed to pull the Unity SDK from\n    its Git URL).\ntransport_requirements:\n- HTTPS is required for all requests.\n- Store access tokens securely.\n- Handle expiration and use refresh tokens.\n- Scope tokens properly to limit access.\nsource_of_requirements: https://developers.sandbox.game/api/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-sand-box/refs/heads/main/authentication/the-sand-box-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Metaverse
- Gaming
- Blockchain
- NFT
- Web3
- Virtual Worlds
- User Generated Content
- Ethereum
- Identity
---
