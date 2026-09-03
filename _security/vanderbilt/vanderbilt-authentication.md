---
api_key_in: []
api_specs:
- filename: vanderbilt-television-news-archive-openapi.yml
  format: yaml
  label: Vanderbilt Television News Archive API
  slug: television-news-archive
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanderbilt/refs/heads/main/openapi/vanderbilt-television-news-archive-openapi.yml
- filename: vanderbilt-sparql-openapi.yml
  format: yaml
  label: Vanderbilt Libraries SPARQL Endpoint
  slug: sparql
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanderbilt/refs/heads/main/openapi/vanderbilt-sparql-openapi.yml
auth_types: []
description: How authentication works across Vanderbilt's institution-operated programmable surfaces. The distinguishing fact for this institution is that its three public read APIs need no credential at all, while everything that touches a person's account runs through Vanderbilt's federated identity estate.
kind: authentication
layout: security
method: probed
name: Vanderbilt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vanderbilt University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Vanderbilt University
provider_slug: vanderbilt
scheme_count: 0
schemes: []
slug: vanderbilt-authentication
source_filename: vanderbilt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nname: Vanderbilt University — Authentication\ndescription: >-\n  How authentication works across Vanderbilt's institution-operated programmable surfaces.\n  The distinguishing fact for this institution is that its three public read APIs need no\n  credential at all, while everything that touches a person's account runs through\n  Vanderbilt's federated identity estate.\ngenerated: '2026-09-01'\nmethod: probed\nsource: Live unauthenticated HTTP probes on 2026-09-01.\nsurfaces:\n  - surface: Vanderbilt Television News Archive API\n    operator: institution\n    base_url: https://7itm2l2dz8.execute-api.us-east-1.amazonaws.com/prod\n    public_read: true\n    scheme: none\n    detail: >-\n      Service root, archive totals, date range, metadata filters, broadcast retrieval and\n      keyword search all returned 200 with no Authorization header and no API key.\n      Personalised operations (/requests, /downloads, /streaming, the /auth/* family)\n      require a signed-in session;\
  \ the application's own error handling raises\n      \"Unauthorized: Please log in to continue\" on 401. Sign-in is either a local account\n      or federated SSO from a subscribing institution — /auth/sso-providers returns the\n      configured domains.\n    evidence:\n      - { url: 'https://7itm2l2dz8.execute-api.us-east-1.amazonaws.com/prod', status: 200 }\n      - { url: 'https://7itm2l2dz8.execute-api.us-east-1.amazonaws.com/prod/auth/sso-providers', status: 200 }\n  - surface: Vanderbilt Libraries SPARQL endpoint\n    operator: institution\n    base_url: https://sparql.vanderbilt.edu/sparql\n    public_read: true\n    scheme: none\n    detail: Query via GET and via direct POST both returned 200 with no credential.\n    evidence:\n      - { url: 'https://sparql.vanderbilt.edu/sparql', status: 200 }\n  - surface: Vanderbilt Institutional Repository (VUIR) — DSpace REST + OAI-PMH\n    operator: institution\n    base_url: https://irbe.library.vanderbilt.edu/server\n    public_read:\
  \ true\n    scheme: none for anonymous read; SAML/Shibboleth for authenticated actions\n    detail: >-\n      The HAL root, community listing and the OAI-PMH request endpoint are open. Deposit,\n      workflow and administrative operations authenticate through the DSpace Shibboleth SP\n      (entityID https://ir.vanderbilt.edu/shibboleth), which redirects to Vanderbilt's Okta\n      IdP at onevu.vanderbilt.edu.\n    evidence:\n      - { url: 'https://irbe.library.vanderbilt.edu/server/api', status: 200 }\n      - { url: 'https://irbe.library.vanderbilt.edu/Shibboleth.sso/Metadata', status: 200 }\n      - { url: 'https://irbe.library.vanderbilt.edu/Shibboleth.sso/DiscoFeed', status: 200 }\nidentity_providers:\n  - name: Vanderbilt Okta (OneVU)\n    operator: federation\n    host: onevu.vanderbilt.edu\n    platform: Okta (custom domain; CNAME -> vanderbilt.customdomains.okta.com)\n    protocols: [OpenID Connect 1.0, OAuth 2.0, SAML 2.0]\n    discovery: https://onevu.vanderbilt.edu/.well-known/openid-configuration\n\
  \    issuer: https://onevu.vanderbilt.edu\n    authorization_endpoint: https://onevu.vanderbilt.edu/oauth2/v1/authorize\n    token_endpoint: https://onevu.vanderbilt.edu/oauth2/v1/token\n    userinfo_endpoint: https://onevu.vanderbilt.edu/oauth2/v1/userinfo\n    jwks_uri: https://onevu.vanderbilt.edu/oauth2/v1/keys\n    registration_endpoint: https://onevu.vanderbilt.edu/oauth2/v1/clients\n    pkce: [S256]\n    token_endpoint_auth_methods:\n      - client_secret_post\n      - client_secret_basic\n      - private_key_jwt\n      - self_signed_tls_client_auth\n    saml_metadata: https://onevu.vanderbilt.edu/app/exk1wcg5n16M91Uyd1d8/sso/saml/metadata\n    saml_entity_id: http://www.okta.com/exk1wcg5n16M91Uyd1d8\n  - name: Vanderbilt Microsoft Entra ID tenant\n    operator: federation\n    domain: vanderbilt.edu\n    tenant_id: ba5a7f39-e3be-4ab3-b450-67fa80faecad\n    protocols: [OpenID Connect 1.0, OAuth 2.0, SAML 2.0, WS-Federation]\n    discovery: https://login.microsoftonline.com/vanderbilt.edu/v2.0/.well-known/openid-configuration\n\
  \    issuer: https://login.microsoftonline.com/ba5a7f39-e3be-4ab3-b450-67fa80faecad/v2.0\n    saml_metadata: https://login.microsoftonline.com/vanderbilt.edu/federationmetadata/2007-06/federationmetadata.xml\n    saml_entity_id: https://sts.windows.net/ba5a7f39-e3be-4ab3-b450-67fa80faecad/\nnotes:\n  - >-\n    InCommon MDQ (https://mdq.incommon.org/entities/{entityID}) returned 404 for\n    urn:mace:incommon:vanderbilt.edu, https://ir.vanderbilt.edu/shibboleth,\n    http://www.okta.com/exk1wcg5n16M91Uyd1d8 and four guessed IdP entityIDs. No InCommon\n    registration was confirmed, so none is claimed here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vanderbilt/refs/heads/main/authentication/vanderbilt-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Private Research University
- Research Data
- Institutional Repository
- Linked Data
- SPARQL
- Digital Collections
- Television News Archive
- Identity Federation
- Library
- Nashville
- Tennessee
- United States
---
