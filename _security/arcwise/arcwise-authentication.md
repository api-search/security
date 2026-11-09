---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Arcwise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arcwise declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Arcwise
provider_slug: arcwise
scheme_count: 1
schemes:
- credential: Personal Access Token created by a user in the admin panel (https://admin.arcwise.app/ > My profile > Personal Access Tokens > + Create)
  header: Authorization
  in: header
  name: personalAccessToken
  note: 'The prose writes "Bearer: <token>" while the documented cURL example sends "Authorization: Bearer <token>" (no colon); the example is the standard RFC 6750 form. The docs say an administrator must create the token for audit-log access. No OAuth scopes are documented for the API.'
  quote: 'Set the `Authorization` header to `Bearer: <your personal access token>` to   authenticate with this endpoint.'
  revocation: At any time, you can click the delete button to permanently revoke a token, at which point it will immediately lose access to Arcwise.
  scheme: bearer
  type: http
slug: arcwise-authentication
source_filename: arcwise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://docs.arcwise.app/arcwise-setup/audit-logging.md\ndocs: https://docs.arcwise.app/arcwise-setup/audit-logging\nschemes:\n- name: personalAccessToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  credential: 'Personal Access Token created by a user in the admin panel (https://admin.arcwise.app/ > My profile > Personal Access Tokens > + Create)'\n  quote: 'Set the `Authorization` header to `Bearer: <your personal access token>` to   authenticate with this endpoint.'\n  revocation: 'At any time, you can click the delete button to permanently revoke a token, at which point it will immediately lose access to Arcwise.'\n  note: 'The prose writes \"Bearer: <token>\" while the documented cURL example sends \"Authorization: Bearer <token>\" (no colon); the example is the standard RFC 6750 form. The docs say an administrator must create the token for audit-log access. No OAuth scopes are documented for\
  \ the API.'\n"
source_yaml_url: https://artifacts.apis.io/arcwise/authentication/arcwise-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Metrics
- Analytics
- Decision-Making
- Business Intelligence
- Root Cause Analysis
---
