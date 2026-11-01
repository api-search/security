---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for the SensorUp GraphQL API
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Sensorup Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: SensorUp Inc. declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: SensorUp Inc.
provider_slug: sensorup-inc
scheme_count: 4
schemes:
- evidence: 'When you sign in through a web browser, the `sensorup_sessionid` cookie is automatically set and sent with each request:'
  how_to_obtain: Obtained after a successful sign‑in mutation; the server sets the `sensorup_sessionid` cookie.
  location: cookie
  name: Session ID (Cookie)
  type: other
- evidence: 'For API clients, mobile apps, and integrations, pass the session ID in the `x-sensorup-sessionid` header:'
  header: x-sensorup-sessionid
  how_to_obtain: Obtained after a successful sign‑in mutation (or API‑key creation); use the returned session ID.
  location: header
  name: Session ID (Header)
  type: other
- evidence: 'Use the API key session ID in the `x-sensorup-sessionid` header (same as regular sessions):'
  header: x-sensorup-sessionid
  how_to_obtain: Create an API key via the `createAPIKey` mutation; the response includes `apiKeySessionId`.
  location: header
  name: API Key Session ID
  type: other
- evidence: 'For organizations using SSO, you can authenticate with Cognito tokens:'
  header: x-sensorup-sessionid
  how_to_obtain: Provide a Cognito ID token to the `federatedSignIn` mutation; the mutation returns a session ID.
  location: header
  name: Federated Sign‑In (Cognito ID Token)
  type: other
slug: sensorup-inc-authentication
source_filename: sensorup-inc-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.sensorup.com/api/graphql/authentication.md
source_yaml: "generated: '2026-10-23'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.sensorup.com/api/graphql/authentication.md\nsources:\n- https://docs.sensorup.com/api/graphql/authentication.md\n- https://docs.sensorup.com/api/graphql/subgraphs/auth.md\n- https://docs.sensorup.com/use-sensorup/getting-started/platform-overview.md\n- https://docs.sensorup.com/use-sensorup/getting-started/building-complete-methane-management-program.md\ndescription: Authentication methods for the SensorUp GraphQL API\nschemes:\n- type: other\n  name: Session ID (Cookie)\n  evidence: 'When you sign in through a web browser, the `sensorup_sessionid` cookie is automatically set and sent with each request:'\n  location: cookie\n  how_to_obtain: Obtained after a successful sign‑in mutation; the server sets the `sensorup_sessionid` cookie.\n- type: other\n  name: Session ID (Header)\n  evidence: 'For API clients, mobile apps, and integrations, pass the session ID in the\
  \ `x-sensorup-sessionid` header:'\n  location: header\n  header: x-sensorup-sessionid\n  how_to_obtain: Obtained after a successful sign‑in mutation (or API‑key creation); use the returned session ID.\n- type: other\n  name: API Key Session ID\n  evidence: 'Use the API key session ID in the `x-sensorup-sessionid` header (same as regular sessions):'\n  location: header\n  header: x-sensorup-sessionid\n  how_to_obtain: Create an API key via the `createAPIKey` mutation; the response includes `apiKeySessionId`.\n- type: other\n  name: Federated Sign‑In (Cognito ID Token)\n  evidence: 'For organizations using SSO, you can authenticate with Cognito tokens:'\n  location: header\n  header: x-sensorup-sessionid\n  how_to_obtain: Provide a Cognito ID token to the `federatedSignIn` mutation; the mutation returns a session ID.\nnote: No OAuth2, HTTP Basic, Bearer, JWT, HMAC, or mTLS schemes are documented on the provided pages.\ndocs: https://docs.sensorup.com/api/graphql/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/sensorup-inc/authentication/sensorup-inc-authentication.yml
summary_line: 4 schemes
tags:
- Company
- IoT
- Industrial
- DataPlatform
- Manufacturing
---
