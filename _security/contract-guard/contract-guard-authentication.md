---
anonymous_access: false
api_key_in: []
auth_types: []
description: Login with Railway uses OAuth 2.0 authorization code flow.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Contract Guard Authentication
name_suffix: Authentication
oauth_flows: []
overview: Contract Guard / Autonomous Utility Factory declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Contract Guard / Autonomous Utility Factory
provider_slug: contract-guard
scheme_count: 1
schemes:
- authorize_url: https://backboard.railway.com/oauth/auth
  evidence: Login with Railway allows third-party applications to authenticate users with their Railway account. Built on OAuth 2.0 and OpenID Connect (OIDC)...
  flows:
  - authorization_code
  how_to_obtain: Create an OAuth app in your workspace's Developer settings to get a client ID and client secret.
  name: Login with Railway
  scopes:
  - openid
  - email
  - profile
  type: oauth2
slug: contract-guard-authentication
source_filename: contract-guard-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.railway.com/access/multi-factor-authentication
source_yaml: "generated: '2026-10-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.railway.com/access/multi-factor-authentication\nsources:\n- https://docs.railway.com/access/multi-factor-authentication\n- https://docs.railway.com/integrations/oauth\n- https://docs.railway.com/integrations/oauth/quickstart\n- https://docs.railway.com/integrations/oauth/creating-an-app\ndescription: Login with Railway uses OAuth 2.0 authorization code flow.\nschemes:\n- type: oauth2\n  name: Login with Railway\n  evidence: Login with Railway allows third-party applications to authenticate users with their Railway account. Built on OAuth 2.0 and OpenID\n    Connect (OIDC)...\n  flows:\n  - authorization_code\n  authorize_url: https://backboard.railway.com/oauth/auth\n  scopes:\n  - openid\n  - email\n  - profile\n  how_to_obtain: Create an OAuth app in your workspace's Developer settings to get a client ID and client secret.\nnote: Token endpoint is https://backboard.railway.com/oauth/token\
  \ as used in the token exchange step.\ndocs: https://docs.railway.com/access/multi-factor-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contract-guard/refs/heads/main/authentication/contract-guard-authentication.yml
summary_line: 1 scheme
tags:
- JSON Validation
- AI Trust
---
