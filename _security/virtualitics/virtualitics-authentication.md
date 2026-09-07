---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Virtualitics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Virtualitics declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Virtualitics
provider_slug: virtualitics
scheme_count: 4
schemes:
- id: vip-auth-token
  in: client-configuration
  issued_by: Virtualitics Account Portal (https://accounts.virtualitics.com) — My Account -> Tokens and Keys -> Generate
  parameter: VIP_AUTH_TOKEN
  presentation: 'Set as the user environment variable VIP_AUTH_TOKEN, or passed positionally when instantiating the handler: `from virtualitics import api; explore = api.VIP(<token>)`.'
  rotation: user-initiated regeneration in the Account Portal; no documented expiry or rotation policy
  scopes: []
  source: https://docs.virtualitics.com/hc/en-us/articles/25103039519635-Setting-up-the-Virtualitics-Python-API-pyVIP-with-Virtualitics-Explore
  surface: Virtualitics Explore Python API (pyVIP)
  transport: WebSocket (Explore server <-> Python client, user-chosen port)
  type: apiKey
- description: '"We strongly recommend using an encryption key. This key is used to encrypt all data passed through the API." Set as a user environment variable alongside VIP_AUTH_TOKEN, or supplied at VIP class instantiation. This is a confidentiality control layered on the WebSocket, distinct from the auth token.'
  id: vip-encryption-key
  in: client-configuration
  parameter: VIP_ENCRYPTION_KEY
  recommended: true
  required: false
  role: payload encryption, not identity
  source: https://docs.virtualitics.com/hc/en-us/articles/25103039519635-Setting-up-the-Virtualitics-Python-API-pyVIP-with-Virtualitics-Explore
  surface: Virtualitics Explore Python API (pyVIP)
  type: shared-secret
- description: '"we will create a configuration file that will hold your API key, username, and host to deploy to." The host is the customer''s own VAIP tenant, e.g. https://abcd.virtualitics.com. The equivalent one-shot form documented in the SDK FAQ is `virtualitics-cli upload dist/<app>.whl --host https://your-platform.com --username <user>`.'
  established_by: '`vaip config`'
  id: vaip-cli-credentials
  in: local-config-file
  parameters:
  - api key
  - username
  - host
  scopes: []
  source: https://docs.virtualitics.com/hc/en-us/articles/34015231987347-Installing-the-Virtualitics-SDK-and-CLI-Packages
  surface: Virtualitics CLI (`vaip`)
  type: apiKey
- description: Platform administrators configure Single Sign-On and password security policy for their tenant. The article documents the administrative capability; it does not publish the protocol, the metadata URL, or any discovery document, and no /.well-known/openid-configuration is served on any Virtualitics host (see well-known/virtualitics-well-known.yml).
  discovery_document: null
  id: platform-sso
  source: https://docs.virtualitics.com/hc/en-us/articles/21926415922323-Setting-Password-Security-and-Configuring-Single-Sign-On-SSO
  surface: Virtualitics AI Platform (human sign-in)
  type: openIdConnect-or-saml
slug: virtualitics-authentication
source_filename: virtualitics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: >-\n  https://docs.virtualitics.com/hc/en-us/articles/25103039519635-Setting-up-the-Virtualitics-Python-API-pyVIP-with-Virtualitics-Explore,\n  https://docs.virtualitics.com/hc/en-us/articles/34015231987347-Installing-the-Virtualitics-SDK-and-CLI-Packages,\n  https://docs.virtualitics.com/hc/en-us/articles/34080541869715-Deploying-an-App-Using-the-Command-Line-Interface-CLI,\n  https://docs.virtualitics.com/hc/en-us/articles/21926415922323-Setting-Password-Security-and-Configuring-Single-Sign-On-SSO\nchecked: '2026-09-04'\nderived_from_spec: false\nspec_note: >-\n  No OpenAPI or other machine-readable contract is published, so no securitySchemes could be\n  derived. Everything below is read from the provider's own documentation.\nsummary: >-\n  Virtualitics authenticates developers with long-lived API tokens minted by the user in the\n  Virtualitics Account Portal, and authenticates human platform users with password or SSO\
  \ against\n  the customer's identity provider. There is no OAuth 2.0 authorization server, no OpenID Connect\n  discovery document, no scope model and no published token endpoint.\nschemes:\n- id: vip-auth-token\n  type: apiKey\n  surface: Virtualitics Explore Python API (pyVIP)\n  in: client-configuration\n  parameter: VIP_AUTH_TOKEN\n  transport: WebSocket (Explore server <-> Python client, user-chosen port)\n  issued_by: Virtualitics Account Portal (https://accounts.virtualitics.com) — My Account -> Tokens and Keys -> Generate\n  presentation: >-\n    Set as the user environment variable VIP_AUTH_TOKEN, or passed positionally when instantiating\n    the handler: `from virtualitics import api; explore = api.VIP(<token>)`.\n  rotation: user-initiated regeneration in the Account Portal; no documented expiry or rotation policy\n  scopes: []\n  source: https://docs.virtualitics.com/hc/en-us/articles/25103039519635-Setting-up-the-Virtualitics-Python-API-pyVIP-with-Virtualitics-Explore\n-\
  \ id: vip-encryption-key\n  type: shared-secret\n  surface: Virtualitics Explore Python API (pyVIP)\n  in: client-configuration\n  parameter: VIP_ENCRYPTION_KEY\n  role: payload encryption, not identity\n  required: false\n  recommended: true\n  description: >-\n    \"We strongly recommend using an encryption key. This key is used to encrypt all data passed\n    through the API.\" Set as a user environment variable alongside VIP_AUTH_TOKEN, or supplied at\n    VIP class instantiation. This is a confidentiality control layered on the WebSocket, distinct\n    from the auth token.\n  source: https://docs.virtualitics.com/hc/en-us/articles/25103039519635-Setting-up-the-Virtualitics-Python-API-pyVIP-with-Virtualitics-Explore\n- id: vaip-cli-credentials\n  type: apiKey\n  surface: Virtualitics CLI (`vaip`)\n  in: local-config-file\n  parameters:\n  - api key\n  - username\n  - host\n  established_by: '`vaip config`'\n  description: >-\n    \"we will create a configuration file that will hold\
  \ your API key, username, and host to deploy\n    to.\" The host is the customer's own VAIP tenant, e.g. https://abcd.virtualitics.com. The\n    equivalent one-shot form documented in the SDK FAQ is\n    `virtualitics-cli upload dist/<app>.whl --host https://your-platform.com --username <user>`.\n  scopes: []\n  source: https://docs.virtualitics.com/hc/en-us/articles/34015231987347-Installing-the-Virtualitics-SDK-and-CLI-Packages\n- id: platform-sso\n  type: openIdConnect-or-saml\n  surface: Virtualitics AI Platform (human sign-in)\n  description: >-\n    Platform administrators configure Single Sign-On and password security policy for their tenant.\n    The article documents the administrative capability; it does not publish the protocol, the\n    metadata URL, or any discovery document, and no /.well-known/openid-configuration is served on\n    any Virtualitics host (see well-known/virtualitics-well-known.yml).\n  discovery_document: null\n  source: https://docs.virtualitics.com/hc/en-us/articles/21926415922323-Setting-Password-Security-and-Configuring-Single-Sign-On-SSO\n\
  oauth2: false\noidc_discovery: false\nscopes_published: false\nmtls: false\nauthorization_model:\n  kind: role and group based, administered in-platform\n  concepts:\n  - users\n  - groups\n  - access levels\n  - user roles\n  - sharing permissions\n  source: https://docs.virtualitics.com/hc/en-us/articles/34964622116499-Exploring-Access-Levels-User-Roles-and-Sharing-Permissions\n  note: >-\n    Documented as platform administration (\"Managing Users\", \"Managing Groups\", \"Exploring Access\n    Levels, User Roles, and Sharing Permissions\"), not as an API authorization scope vocabulary.\ngaps:\n- No token expiry, lifetime or rotation policy is published for VIP_AUTH_TOKEN.\n- No scope or least-privilege model exists for either the pyVIP token or the CLI API key.\n- No machine-readable discovery document (OIDC or OAuth) is served on any host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtualitics/refs/heads/main/authentication/virtualitics-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Artificial Intelligence
- Data Analytics
- Data Visualization
- Machine Learning
- Defense
- Government
- Python
- SDK
- Command Line Interface
---
