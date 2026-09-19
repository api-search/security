---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: bugsnag-builds-api-openapi.yml
  format: yaml
  label: bugsnag Builds API
  slug: bugsnag-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-builds-api-openapi.yml
- filename: bugsnag-collaborators-api-openapi.yml
  format: yaml
  label: bugsnag Collaborators API
  slug: bugsnag-collaborators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-collaborators-api-openapi.yml
- filename: bugsnag-comments-api-openapi.yml
  format: yaml
  label: bugsnag Comments API
  slug: bugsnag-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-comments-api-openapi.yml
- filename: bugsnag-errors-api-openapi.yml
  format: yaml
  label: bugsnag Errors API
  slug: bugsnag-errors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-errors-api-openapi.yml
- filename: bugsnag-eventfields-api-openapi.yml
  format: yaml
  label: bugsnag EventFields API
  slug: bugsnag-eventfields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-eventfields-api-openapi.yml
- filename: bugsnag-events-api-openapi.yml
  format: yaml
  label: bugsnag Events API
  slug: bugsnag-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-events-api-openapi.yml
- filename: bugsnag-organizations-api-openapi.yml
  format: yaml
  label: bugsnag Organizations API
  slug: bugsnag-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-organizations-api-openapi.yml
- filename: bugsnag-pivots-api-openapi.yml
  format: yaml
  label: bugsnag Pivots API
  slug: bugsnag-pivots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-pivots-api-openapi.yml
- filename: bugsnag-projects-api-openapi.yml
  format: yaml
  label: bugsnag Projects API
  slug: bugsnag-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-projects-api-openapi.yml
- filename: bugsnag-releases-api-openapi.yml
  format: yaml
  label: bugsnag Releases API
  slug: bugsnag-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-releases-api-openapi.yml
- filename: bugsnag-sessions-api-openapi.yml
  format: yaml
  label: bugsnag Sessions API
  slug: bugsnag-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-sessions-api-openapi.yml
- filename: bugsnag-stability-api-openapi.yml
  format: yaml
  label: bugsnag Stability API
  slug: bugsnag-stability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-stability-api-openapi.yml
- filename: bugsnag-traces-api-openapi.yml
  format: yaml
  label: bugsnag Traces API
  slug: bugsnag-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-traces-api-openapi.yml
- filename: bugsnag-trends-api-openapi.yml
  format: yaml
  label: bugsnag Trends API
  slug: bugsnag-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-trends-api-openapi.yml
- filename: bugsnag-current-user-api-openapi.yml
  format: yaml
  label: Bugsnag Current User API
  slug: bugsnag-current-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-current-user-api-openapi.yml
- filename: bugsnag-error-reporting-api-openapi.json
  format: json
  label: BugSnag Error Reporting API
  slug: bugsnag-error-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-error-reporting-api-openapi.json
- filename: bugsnag-upload-api-openapi.json
  format: json
  label: BugSnag Upload API
  slug: bugsnag-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-upload-api-openapi.json
auth_types:
- apiKey
- http
- oauth2
description: 'BugSnag has three distinct authentication models, one per surface class: a personal auth token for the Data Access API, a project API key for the ingest and upload endpoints, and OAuth 2.1 for the remote MCP server.'
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Bugsnag Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bugsnag secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bugsnag
provider_slug: bugsnag
scheme_count: 4
schemes:
- description: 'Personal Auth Token, the recommended and default method. Generated in the dashboard''s account settings. Verbatim from the spec: "Authorize using a Personal Auth Token with the `token` prefix, e.g. \"token my_auth_token\"."'
  format: token YOUR-AUTH-TOKEN
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/bugsnag-data-access-api-openapi.json
  - https://developer.smartbear.com/bugsnag/docs/data-access-authentication
  surface: Data Access API (https://api.bugsnag.com)
  type: apiKey
- description: On-premise installations may authenticate with dashboard user credentials (the email address and password of the user) via HTTP Basic. The docs state this is for on-premise only; SaaS callers use a personal auth token.
  name: basicAuth
  scheme: basic
  sources:
  - https://developer.smartbear.com/bugsnag/docs/data-access-authentication
  surface: Data Access API — on-premise installations only
  type: http
- carriers:
  - in: header
    note: Optional (required:false in the spec) on 'POST https://sessions.bugsnag.com/'.
    parameter: Bugsnag-Api-Key
    required: true
    surfaces:
    - POST https://notify.bugsnag.com/ (Error Reporting)
    - POST https://otlp.bugsnag.com/traces/v1 (Trace)
  - in: query
    note: The remaining Upload API endpoints take the key in the multipart form body rather than as a declared parameter.
    parameter: api_key
    required: true
    surfaces:
    - POST https://notify.bugsnag.com/minidump
    - POST https://upload.bugsnag.com/breakpad-symbol
  description: Per-project API key identifying which BugSnag project an event, session, build, span or symbol file belongs to. It is an ingest identifier, not a user credential — it is shipped inside client applications. None of the ingest specs declare a securitySchemes block; the key travels as an explicit parameter instead. Rotatable via the Data Access API (regenerateProjectApiKey, regenerateProjectUploadApiKey).
  in: header-or-query-or-body
  name: projectApiKey
  sources:
  - openapi/bugsnag-error-reporting-api-openapi.json
  - openapi/bugsnag-upload-api-openapi.json
  - openapi/bugsnag-trace-api-openapi.json
  - openapi/bugsnag-session-tracking-api-openapi.json
  surface: Error Reporting (notify.bugsnag.com), Session Tracking (sessions.bugsnag.com), Build (build.bugsnag.com), Trace (otlp.bugsnag.com) and Upload (upload.bugsnag.com) APIs
  type: apiKey
- description: Browser-based OAuth login for the hosted MCP server, added in May 2026 per the BugSnag changelog ("Self Hosted MCP Server OAuth 2.0 support — securely connect to BugSnag via browser-based login instead of manual API tokens"). The server also accepts a Bugsnag-Auth-Token header as an alternative.
  dynamic_client_registration: https://oauth.bugsnag.com/register
  flows:
    authorizationCode:
      authorizationUrl: https://oauth.bugsnag.com/authorize
      scopes:
        api: Access the BugSnag API on behalf of the user
        openid: OIDC sign-in
        profile: OIDC profile claims
      tokenUrl: https://oauth.bugsnag.com/token
  name: oauth2
  pkce: S256
  sources:
  - https://oauth.bugsnag.com/.well-known/oauth-authorization-server
  - https://bugsnag.mcp.smartbear.com/.well-known/oauth-protected-resource
  - https://docs.bugsnag.com/whats-new/
  surface: BugSnag remote MCP server (https://bugsnag.mcp.smartbear.com/mcp)
  type: oauth2
slug: bugsnag-authentication
source_filename: bugsnag-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: >-\n  https://developer.smartbear.com/bugsnag/docs/data-access-authentication ,\n  openapi/bugsnag-data-access-api-openapi.json (securitySchemes) ,\n  https://oauth.bugsnag.com/.well-known/oauth-authorization-server\ndocs: https://developer.smartbear.com/bugsnag/docs/data-access-authentication\nsummary:\n  types:\n    - apiKey\n    - http\n    - oauth2\n  api_key_in:\n    - header\ndescription: >-\n  BugSnag has three distinct authentication models, one per surface class: a\n  personal auth token for the Data Access API, a project API key for the ingest\n  and upload endpoints, and OAuth 2.1 for the remote MCP server.\nschemes:\n  - name: tokenAuth\n    surface: Data Access API (https://api.bugsnag.com)\n    type: apiKey\n    in: header\n    parameter: Authorization\n    format: 'token YOUR-AUTH-TOKEN'\n    description: >-\n      Personal Auth Token, the recommended and default method. Generated in the\n      dashboard's account\
  \ settings. Verbatim from the spec: \"Authorize using a\n      Personal Auth Token with the `token` prefix, e.g. \\\"token my_auth_token\\\".\"\n    sources:\n      - openapi/bugsnag-data-access-api-openapi.json\n      - https://developer.smartbear.com/bugsnag/docs/data-access-authentication\n  - name: basicAuth\n    surface: Data Access API — on-premise installations only\n    type: http\n    scheme: basic\n    description: >-\n      On-premise installations may authenticate with dashboard user credentials\n      (the email address and password of the user) via HTTP Basic. The docs\n      state this is for on-premise only; SaaS callers use a personal auth token.\n    sources:\n      - https://developer.smartbear.com/bugsnag/docs/data-access-authentication\n  - name: projectApiKey\n    surface: >-\n      Error Reporting (notify.bugsnag.com), Session Tracking\n      (sessions.bugsnag.com), Build (build.bugsnag.com), Trace\n      (otlp.bugsnag.com) and Upload (upload.bugsnag.com) APIs\n\
  \    type: apiKey\n    in: header-or-query-or-body\n    carriers:\n      - parameter: Bugsnag-Api-Key\n        in: header\n        required: true\n        surfaces:\n          - 'POST https://notify.bugsnag.com/ (Error Reporting)'\n          - 'POST https://otlp.bugsnag.com/traces/v1 (Trace)'\n        note: >-\n          Optional (required:false in the spec) on\n          'POST https://sessions.bugsnag.com/'.\n      - parameter: api_key\n        in: query\n        required: true\n        surfaces:\n          - 'POST https://notify.bugsnag.com/minidump'\n          - 'POST https://upload.bugsnag.com/breakpad-symbol'\n        note: >-\n          The remaining Upload API endpoints take the key in the multipart form\n          body rather than as a declared parameter.\n    description: >-\n      Per-project API key identifying which BugSnag project an event, session,\n      build, span or symbol file belongs to. It is an ingest identifier, not a\n      user credential — it is shipped inside\
  \ client applications. None of the\n      ingest specs declare a securitySchemes block; the key travels as an\n      explicit parameter instead. Rotatable via the Data Access API\n      (regenerateProjectApiKey, regenerateProjectUploadApiKey).\n    sources:\n      - openapi/bugsnag-error-reporting-api-openapi.json\n      - openapi/bugsnag-upload-api-openapi.json\n      - openapi/bugsnag-trace-api-openapi.json\n      - openapi/bugsnag-session-tracking-api-openapi.json\n  - name: oauth2\n    surface: BugSnag remote MCP server (https://bugsnag.mcp.smartbear.com/mcp)\n    type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://oauth.bugsnag.com/authorize\n        tokenUrl: https://oauth.bugsnag.com/token\n        scopes:\n          api: Access the BugSnag API on behalf of the user\n          openid: OIDC sign-in\n          profile: OIDC profile claims\n    pkce: S256\n    dynamic_client_registration: https://oauth.bugsnag.com/register\n    description: >-\n  \
  \    Browser-based OAuth login for the hosted MCP server, added in May 2026 per\n      the BugSnag changelog (\"Self Hosted MCP Server OAuth 2.0 support — securely\n      connect to BugSnag via browser-based login instead of manual API tokens\").\n      The server also accepts a Bugsnag-Auth-Token header as an alternative.\n    sources:\n      - https://oauth.bugsnag.com/.well-known/oauth-authorization-server\n      - https://bugsnag.mcp.smartbear.com/.well-known/oauth-protected-resource\n      - https://docs.bugsnag.com/whats-new/\ntoken_management:\n  rotation:\n    - operationId: revokeOrganizationAuthToken\n      path: DELETE /organizations/{id}/auth_token\n    - operationId: revokeOrganizationApiKey\n      path: DELETE /organizations/{id}/api_key\n    - operationId: regenerateProjectApiKey\n      path: DELETE /projects/{project_id}/api_key\n    - operationId: regenerateProjectUploadApiKey\n      path: DELETE /projects/{project_id}/upload_api_key\n  note: >-\n    Both organization-level\
  \ and project-level credentials can be revoked or\n    regenerated programmatically — unusual, and a genuine agent-safety feature.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/authentication/bugsnag-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Monitoring
- Observability
- Error Monitoring
- Application Performance Monitoring
- Distributed Tracing
- Developer Tools
- SmartBear
---
