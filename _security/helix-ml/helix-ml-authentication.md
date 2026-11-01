---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods published for HelixML services
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Helix Ml Authentication
name_suffix: Authentication
oauth_flows: []
overview: HelixML declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: HelixML
provider_slug: helix-ml
scheme_count: 2
schemes:
- evidence: Helix supports OpenID Connect (OIDC) for integration with external identity providers like Okta, Auth0, Azure AD, or Google.
  flows:
  - authorization_code
  how_to_obtain: Configure your OIDC provider using environment variables such as OIDC_URL, OIDC_CLIENT_ID, OIDC_CLIENT_SECRET, etc.
  name: Custom OIDC Provider
  scopes:
  - openid
  - profile
  - email
  type: oauth2
- evidence: 'Ramjet accepts it as Authorization: Bearer ...'
  header: Authorization
  how_to_obtain: Create a token via Ramjet's management API using the dashboard's admin token.
  location: header
  name: Ramjet Bearer Token
  type: http-bearer
slug: helix-ml-authentication
source_filename: helix-ml-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.helixml.tech/helix/private-deployment/oidc/
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.helixml.tech/helix/private-deployment/oidc/\nsources:\n- https://docs.helixml.tech/helix/private-deployment/oidc/\n- https://helix.ml/blog/ramjet-api-tokens-and-usage-accounting\n- https://helix.ml/blog/basalt-qwen38-flash-next-rtx-pro-6000\n- https://helix.ml/blog/swift-flash-next-four-gpu-evaluation\ndescription: Authentication methods published for HelixML services\nschemes:\n- type: oauth2\n  name: Custom OIDC Provider\n  evidence: Helix supports OpenID Connect (OIDC) for integration with external identity providers like Okta, Auth0, Azure AD, or Google.\n  flows:\n  - authorization_code\n  scopes:\n  - openid\n  - profile\n  - email\n  how_to_obtain: Configure your OIDC provider using environment variables such as OIDC_URL, OIDC_CLIENT_ID, OIDC_CLIENT_SECRET, etc.\n- type: http-bearer\n  name: Ramjet Bearer Token\n  evidence: 'Ramjet accepts it as Authorization:\
  \ Bearer ...'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a token via Ramjet's management API using the dashboard's admin token.\ndocs: https://docs.helixml.tech/helix/private-deployment/oidc/\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/helix-ml/authentication/helix-ml-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Agent Virtualization
- Security
- Cloud
---
