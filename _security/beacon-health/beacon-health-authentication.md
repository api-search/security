---
api_key_in: []
auth_types:
- openIdConnect
description: Beacon Health publishes no public developer API and no OpenAPI definition, so there are no securitySchemes to derive from. This profile is captured from the live OIDC discovery document served by the application backend host (api.beaconhealth.ai) plus the published Terms of Service and Privacy Policy. The discovery document advertises an issuer and a working JWKS endpoint, which indicates JWT-based session authentication for the first-party Beacon Health web application; the advertised authorization_endpoint returns 404, so this is NOT a public OAuth authorization server that third-party developers can register with. Human end users authenticate through the web application at https://www.beaconhealth.ai/login. Access to the platform requires authorization by a subscribing healthcare organization (Terms of Service §3).
kind: authentication
layout: security
method: searched
name: Beacon Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Beacon Health secures its APIs with openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Beacon Health
provider_slug: beacon-health
scheme_count: 1
schemes:
- authorization_endpoint: https://api.beaconhealth.ai/oauth/authorize
  authorization_endpoint_status: 404
  issuer: https://api.beaconhealth.ai
  jwks_algorithms:
  - RSA
  jwks_keys: 1
  jwks_uri: https://api.beaconhealth.ai/.well-known/jwks.json
  name: BeaconHealthApplicationJWT
  scopes_advertised: []
  sources:
  - well-known/beacon-health-openid-configuration.json
  - well-known/beacon-health-jwks.json
  token_endpoint: null
  type: openIdConnect
slug: beacon-health-authentication
source_filename: beacon-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.beaconhealth.ai/.well-known/openid-configuration\ndescription: >-\n  Beacon Health publishes no public developer API and no OpenAPI definition, so\n  there are no securitySchemes to derive from. This profile is captured from the\n  live OIDC discovery document served by the application backend host\n  (api.beaconhealth.ai) plus the published Terms of Service and Privacy Policy.\n  The discovery document advertises an issuer and a working JWKS endpoint, which\n  indicates JWT-based session authentication for the first-party Beacon Health\n  web application; the advertised authorization_endpoint returns 404, so this is\n  NOT a public OAuth authorization server that third-party developers can\n  register with. Human end users authenticate through the web application at\n  https://www.beaconhealth.ai/login. Access to the platform requires\n  authorization by a subscribing healthcare organization (Terms of Service §3).\n\
  summary:\n  types:\n    - openIdConnect\n  public_developer_auth: false\n  self_serve_signup: false\n  notes: >-\n    First-party application authentication only. No documented API keys, no\n    published OAuth client registration, no developer credentials.\nschemes:\n  - name: BeaconHealthApplicationJWT\n    type: openIdConnect\n    issuer: https://api.beaconhealth.ai\n    jwks_uri: https://api.beaconhealth.ai/.well-known/jwks.json\n    jwks_keys: 1\n    jwks_algorithms:\n      - RSA\n    authorization_endpoint: https://api.beaconhealth.ai/oauth/authorize\n    authorization_endpoint_status: 404\n    token_endpoint: null\n    scopes_advertised: []\n    sources:\n      - well-known/beacon-health-openid-configuration.json\n      - well-known/beacon-health-jwks.json\nhuman_login: https://www.beaconhealth.ai/login\naccess_control:\n  model: organization-provisioned\n  evidence: >-\n    \"To use our Services, you must be at least 18 years old and authorized by a\n    subscribing healthcare\
  \ organization.\" — Terms of Service §3,\n    https://www.beaconhealth.ai/terms\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beacon-health/refs/heads/main/authentication/beacon-health-authentication.yml
summary_line: openIdConnect · 1 scheme
tags:
- Company
- Healthcare
- Primary Care
- Value Based Care
- EHR
- Artificial Intelligence
- AI Agents
- Workflow Automation
- Risk Adjustment
- Prior Authorization
- HIPAA
- Y Combinator
---
