---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for AiESphere
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Aiesphere Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: AiESphere declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: AiESphere
provider_slug: aiesphere-com
scheme_count: 3
schemes:
- authorize_url: https://aiesphere.com/api/mcp/authorize
  evidence: '"grant_types_supported":["authorization_code","refresh_token"]'
  flows:
  - authorization_code
  name: OAuth2
  scopes:
  - openid
  - profile
  - email
  - offline_access
  - jobs.read
  - jobs.write
  - profile.read
  - profile.write
  - applications.read
  - applications.write
  - resume.tailor
  - cover.generate
  - apply.submit
  type: oauth2
- evidence: '"token_endpoint_auth_methods_supported":["client_secret_basic","client_secret_post","none"]'
  header: Authorization
  location: header
  name: client_secret_basic
  type: http-basic
- evidence: '"token_endpoint_auth_methods_supported":["client_secret_basic","client_secret_post","none"]'
  location: body
  name: client_secret_post
  type: other
slug: aiesphere-com-authentication
source_filename: aiesphere-com-authentication.yml
source_heading: Authentication Profile
source_url: https://aiesphere.com/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://aiesphere.com/.well-known/oauth-authorization-server\nsources:\n- https://aiesphere.com/.well-known/oauth-authorization-server\n- https://aiesphere.com/.well-known/oauth-protected-resource\ndescription: Authentication methods for AiESphere\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: '\"grant_types_supported\":[\"authorization_code\",\"refresh_token\"]'\n  flows:\n  - authorization_code\n  authorize_url: https://aiesphere.com/api/mcp/authorize\n  scopes:\n  - openid\n  - profile\n  - email\n  - offline_access\n  - jobs.read\n  - jobs.write\n  - profile.read\n  - profile.write\n  - applications.read\n  - applications.write\n  - resume.tailor\n  - cover.generate\n  - apply.submit\n- type: http-basic\n  name: client_secret_basic\n  evidence: '\"token_endpoint_auth_methods_supported\":[\"client_secret_basic\",\"client_secret_post\",\"none\"]'\n  location: header\n\
  \  header: Authorization\n- type: other\n  name: client_secret_post\n  evidence: '\"token_endpoint_auth_methods_supported\":[\"client_secret_basic\",\"client_secret_post\",\"none\"]'\n  location: body\ndocs: https://aiesphere.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/aiesphere-com/authentication/aiesphere-com-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- Careers
- Education
- Platform
- India
---
