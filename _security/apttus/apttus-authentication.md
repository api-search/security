---
anonymous_access: false
api_key_in: []
auth_types: []
description: Conga’s REST API authentication requires a bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Apttus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apttus declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Apttus
provider_slug: apttus
scheme_count: 1
schemes:
- evidence: Conga’s REST API authentication requires a bearer token.
  header: Authorization
  how_to_obtain: Generate an authentication token via the Auth Access Token API call using client_id and client_secret with grant_type 'client_credentials'.
  location: header
  name: Authorization
  token_url: https://login-rls.congacloud.com/api/v1/auth/connect/token
  type: http-bearer
slug: apttus-authentication
source_filename: apttus-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.conga.com/platform/reference/authentication.md
source_yaml: "generated: '2026-09-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.conga.com/platform/reference/authentication.md\nsources:\n- https://developer.conga.com/platform/reference/authentication.md\n- https://developer.conga.com/platform/reference/post_api-external-endpoint-config-v1-credentials-1.md\n- https://developer.conga.com/platform/reference/put_api-external-endpoint-config-v1-credentials-1.md\n- https://developer.conga.com/platform/reference/get_api-external-endpoint-config-v1-credentials-name-1.md\ndescription: Conga’s REST API authentication requires a bearer token.\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: Conga’s REST API authentication requires a bearer token.\n  location: header\n  header: Authorization\n  token_url: https://login-rls.congacloud.com/api/v1/auth/connect/token\n  how_to_obtain: Generate an authentication token via the Auth Access Token API call using client_id and client_secret\
  \ with grant_type 'client_credentials'.\ndocs: https://developer.conga.com/platform/reference/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apttus/refs/heads/main/authentication/apttus-authentication.yml
summary_line: 1 scheme
tags:
- Software-as-a-Service
- CPQ
- Contract Lifecycle Management
- Document Automation
- Quote-to-Cash
- Company
---
