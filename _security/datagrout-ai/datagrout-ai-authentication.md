---
anonymous_access: false
api_key_in: []
api_specs:
- filename: datagrout-ai-openapi-generated.yml
  format: yaml
  label: DataGrout API
  slug: datagrout-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagrout-ai/openapi/_ae-authored/datagrout-ai-openapi-generated.yml
auth_types: []
description: 'DataGrout supports three authentication methods: access tokens (Bearer), mutual TLS (mTLS), and OAuth 2.1.'
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Datagrout Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: DataGrout declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: DataGrout
provider_slug: datagrout-ai
scheme_count: 3
schemes:
- evidence: The simplest method. Create a token in the UI, pass it in the Authorization header.
  header: Authorization
  how_to_obtain: 'Create a token in the UI: Settings > Authentication > Create Access Token, then copy the token.'
  location: header
  name: Access Token
  type: http-bearer
- evidence: Certificate-based authentication for production deployments. The client certificate is the credential – no bearer token needed after the initial bootstrap.
  how_to_obtain: Bootstrap identity with a token or OAuth client_credentials via the Conduit SDK, which generates a DG‑signed certificate stored in ~/.conduit/.
  location: tls
  name: Mutual TLS
  type: mtls
- evidence: For user‑facing applications where users delegate access to your agent.
  header: Authorization
  how_to_obtain: Create an OAuth client in Settings > Authentication, then use either the Client Credentials flow (POST to the token URL with grant_type=client_credentials, client_id, client_secret) or the Authorization Code flow (redirect user to the DataGrout authorization endpoint, then exchange code for token).
  location: header
  name: OAuth 2.1
  token_url: https://gateway.datagrout.ai/oauth/token
  type: oauth2
slug: datagrout-ai-authentication
source_filename: datagrout-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://datagrout.ai/oauth/consent
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://datagrout.ai/oauth/consent\nsources:\n- https://datagrout.ai/oauth/consent\n- https://docs.datagrout.ai/authentication\n- https://datagrout.ai/solutions/ai-cost-optimization\n- https://datagrout.ai/case-studies/context-hydration\ndescription: 'DataGrout supports three authentication methods: access tokens (Bearer), mutual TLS (mTLS), and OAuth 2.1.'\nschemes:\n- type: http-bearer\n  name: Access Token\n  evidence: The simplest method. Create a token in the UI, pass it in the Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: 'Create a token in the UI: Settings > Authentication > Create Access Token, then copy the token.'\n- type: mtls\n  name: Mutual TLS\n  evidence: Certificate-based authentication for production deployments. The client certificate is the credential – no bearer token needed after\n    the initial bootstrap.\n  location:\
  \ tls\n  how_to_obtain: Bootstrap identity with a token or OAuth client_credentials via the Conduit SDK, which generates a DG‑signed certificate stored\n    in ~/.conduit/.\n- type: oauth2\n  name: OAuth 2.1\n  evidence: For user‑facing applications where users delegate access to your agent.\n  location: header\n  header: Authorization\n  token_url: https://gateway.datagrout.ai/oauth/token\n  how_to_obtain: Create an OAuth client in Settings > Authentication, then use either the Client Credentials flow (POST to the token URL with\n    grant_type=client_credentials, client_id, client_secret) or the Authorization Code flow (redirect user to the DataGrout authorization endpoint,\n    then exchange code for token).\ndocs: https://datagrout.ai/oauth/consent\n"
source_yaml_url: https://artifacts.apis.io/datagrout-ai/authentication/datagrout-ai-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- Enterprise
- Platform
- Memory
- Tools
---
