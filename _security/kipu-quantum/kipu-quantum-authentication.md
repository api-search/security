---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Kipu Quantum Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Kipu Quantum secures its APIs with apiKey, oauth2, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Kipu Quantum
provider_slug: kipu-quantum
scheme_count: 2
schemes:
- description: First-party API key issued from the Hub, passed by the Python SDK / REST API (api_key="..."). Available on the Plus tier and above.
  in: header
  name: apiKey
  source: https://kipu-quantum.com/platform
  type: apiKey
- description: Keycloak OpenID Connect provider (PlanQK realm) that fronts the Hub. Issues OAuth2 access tokens via authorization_code (interactive) and client_credentials (service accounts).
  name: oidc
  openIdConnectUrl: https://login.hub.kipu-quantum.com/realms/planqk/.well-known/openid-configuration
  source: https://login.hub.kipu-quantum.com/realms/planqk/.well-known/openid-configuration
  type: openIdConnect
slug: kipu-quantum-authentication
source_filename: kipu-quantum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://kipu-quantum.com/platform\ndocs: https://login.hub.kipu-quantum.com/realms/planqk/.well-known/openid-configuration\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, clientCredentials]\n  notes: >-\n    The Kipu Quantum Hub REST API and Python SDK authenticate with an API key\n    (shown in SDK examples as api_key=\"...\"). Interactive and machine-to-machine\n    access to the platform is brokered by a Keycloak OpenID Connect provider\n    (PlanQK realm) supporting the authorization_code and client_credentials\n    grants. Derived by inspection of the platform docs and the live OIDC\n    discovery document; no OpenAPI is published yet (v1 SDK docs pending).\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  description: >-\n    First-party API key issued from the Hub, passed by the Python SDK / REST API\n    (api_key=\"...\"). Available on the Plus\
  \ tier and above.\n  source: https://kipu-quantum.com/platform\n- name: oidc\n  type: openIdConnect\n  openIdConnectUrl: https://login.hub.kipu-quantum.com/realms/planqk/.well-known/openid-configuration\n  description: >-\n    Keycloak OpenID Connect provider (PlanQK realm) that fronts the Hub. Issues\n    OAuth2 access tokens via authorization_code (interactive) and\n    client_credentials (service accounts).\n  source: https://login.hub.kipu-quantum.com/realms/planqk/.well-known/openid-configuration\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kipu-quantum/refs/heads/main/authentication/kipu-quantum-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 2 schemes
tags:
- Company
- Deep Tech
- Quantum Computing
- Quantum
- Artificial Intelligence
- Optimization
- Developer Platform
- SDK
- REST API
- Germany
---
