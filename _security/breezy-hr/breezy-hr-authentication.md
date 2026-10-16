---
anonymous_access: false
api_key_in: []
api_specs:
- filename: breezy-hr-openapi-generated.yml
  format: yaml
  label: Breezy HR API
  slug: breezy-hr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breezy-hr/refs/heads/main/openapi/_ae-authored/breezy-hr-openapi-generated.yml
auth_types: []
description: Breezy HR API authentication
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Breezy Hr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Breezy HR declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Breezy HR
provider_slug: breezy-hr
scheme_count: 2
schemes:
- evidence: All requests (except /v3/signin and /v3/health) require an Authorization header.
  header: Authorization
  how_to_obtain: 'Create a PAT in the Breezy app: click your user icon → My Settings → API Keys tab → Create API Key, then copy the token.'
  location: header
  name: Personal Access Token
  type: apiKey
- evidence: 'Obtain a session token by calling POST /v3/signin with your email and password. The returned access_token is used the same way:'
  header: Authorization
  how_to_obtain: POST https://api.breezy.hr/v3/signin with email and password to receive an access_token.
  location: header
  name: Session Token
  type: apiKey
slug: breezy-hr-authentication
source_filename: breezy-hr-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.breezy.hr/reference/authorization
source_yaml: "generated: '2026-10-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.breezy.hr/reference/authorization\nsources:\n- https://developer.breezy.hr/reference/authorization\n- https://help.breezy.hr/en/articles/13941514-multi-factor-authentication\n- https://developer.breezy.hr/reference/signin-1\n- https://developer.breezy.hr/reference/signin-1\ndescription: Breezy HR API authentication\nschemes:\n- type: apiKey\n  name: Personal Access Token\n  evidence: All requests (except /v3/signin and /v3/health) require an Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: 'Create a PAT in the Breezy app: click your user icon → My Settings → API Keys tab → Create API Key, then copy the token.'\n- type: apiKey\n  name: Session Token\n  evidence: 'Obtain a session token by calling POST /v3/signin with your email and password. The returned access_token is used the same way:'\n  location: header\n  header: Authorization\n\
  \  how_to_obtain: POST https://api.breezy.hr/v3/signin with email and password to receive an access_token.\nnote: Both methods use the Authorization header; no OAuth2 flows are documented.\ndocs: https://developer.breezy.hr/reference/authorization\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breezy-hr/refs/heads/main/authentication/breezy-hr-authentication.yml
summary_line: 2 schemes
tags:
- Hiring
- ATS
- Recruitment
- SaaS
- HRTech
---
