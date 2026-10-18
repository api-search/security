---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods supported by ApyGuard as described in the documentation.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Apyguard Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apyguard declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Apyguard
provider_slug: apyguard
scheme_count: 3
schemes:
- evidence: Use an existing API key, bearer token, or similar credential in ApyGuard for protected endpoint testing.
  name: Predefined Token
  type: apiKey
- evidence: Login URL authentication allows ApyGuard to log in using a real API endpoint, retrieve a token from the response, and then use that token for protected endpoint testing.
  name: Login URL
  type: other
- evidence: Use OIDC when your identity provider exposes OpenID Connect discovery metadata and your API relies on that provider for authentication.
  name: OIDC
  type: oauth2
slug: apyguard-authentication
source_filename: apyguard-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.apyguard.com/authentication/overview.md
source_yaml: "generated: '2026-10-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.apyguard.com/authentication/overview.md\nsources:\n- https://docs.apyguard.com/authentication/overview.md\n- https://docs.apyguard.com/authentication/predefined-token.md\n- https://docs.apyguard.com/authentication/login-url.md\n- https://docs.apyguard.com/authentication/oidc.md\ndescription: Authentication methods supported by ApyGuard as described in the documentation.\nschemes:\n- type: apiKey\n  name: Predefined Token\n  evidence: Use an existing API key, bearer token, or similar credential in ApyGuard for protected endpoint testing.\n- type: other\n  name: Login URL\n  evidence: Login URL authentication allows ApyGuard to log in using a real API endpoint, retrieve a token from the response, and then use that\n    token for protected endpoint testing.\n- type: oauth2\n  name: OIDC\n  evidence: Use OIDC when your identity provider exposes OpenID Connect discovery\
  \ metadata and your API relies on that provider for authentication.\ndocs: https://docs.apyguard.com/authentication/overview.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apyguard/refs/heads/main/authentication/apyguard-authentication.yml
summary_line: 3 schemes
tags:
- Company
- API Security
- Developer Tools
- Software-as-a-Service
- Cloud
---
