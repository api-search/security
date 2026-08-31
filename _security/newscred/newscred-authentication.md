---
api_key_in: []
api_specs:
- filename: newscred-assets-api-openapi.yml
  format: yaml
  label: Newscred Assets API
  slug: newscred-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/openapi/newscred-assets-api-openapi.yml
- filename: newscred-brand-compliance-api-openapi.yml
  format: yaml
  label: Newscred Brand Compliance API
  slug: newscred-brand-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/openapi/newscred-brand-compliance-api-openapi.yml
- filename: newscred-campaigns-api-openapi.yml
  format: yaml
  label: Newscred Campaigns API
  slug: newscred-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/openapi/newscred-campaigns-api-openapi.yml
- filename: newscred-events-api-openapi.yml
  format: yaml
  label: Newscred Events API
  slug: newscred-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/openapi/newscred-events-api-openapi.yml
- filename: newscred-fields-api-openapi.yml
  format: yaml
  label: Newscred Fields API
  slug: newscred-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/openapi/newscred-fields-api-openapi.yml
- filename: newscred-labels-api-openapi.yml
  format: yaml
  label: Newscred Labels API
  slug: newscred-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/openapi/newscred-labels-api-openapi.yml
- filename: newscred-library-api-openapi.yml
  format: yaml
  label: Newscred Library API
  slug: newscred-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/openapi/newscred-library-api-openapi.yml
- filename: newscred-milestones-api-openapi.yml
  format: yaml
  label: Newscred Milestones API
  slug: newscred-milestones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/openapi/newscred-milestones-api-openapi.yml
- filename: newscred-publishing-api-openapi.yml
  format: yaml
  label: Newscred Publishing API
  slug: newscred-publishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/openapi/newscred-publishing-api-openapi.yml
- filename: newscred-settings-api-openapi.yml
  format: yaml
  label: Newscred Settings API
  slug: newscred-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/openapi/newscred-settings-api-openapi.yml
- filename: newscred-structured-contents-api-openapi.yml
  format: yaml
  label: Newscred Structured Contents API
  slug: newscred-structured-contents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/openapi/newscred-structured-contents-api-openapi.yml
- filename: newscred-task-step-api-openapi.yml
  format: yaml
  label: Newscred Task Step API
  slug: newscred-task-step-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/openapi/newscred-task-step-api-openapi.yml
- filename: newscred-tasks-api-openapi.yml
  format: yaml
  label: Newscred Tasks API
  slug: newscred-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/openapi/newscred-tasks-api-openapi.yml
- filename: newscred-teams-api-openapi.yml
  format: yaml
  label: Newscred Teams API
  slug: newscred-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/openapi/newscred-teams-api-openapi.yml
- filename: newscred-templates-api-openapi.yml
  format: yaml
  label: Newscred Templates API
  slug: newscred-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/openapi/newscred-templates-api-openapi.yml
- filename: newscred-uploader-api-openapi.yml
  format: yaml
  label: Newscred Uploader API
  slug: newscred-uploader-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/openapi/newscred-uploader-api-openapi.yml
- filename: newscred-users-api-openapi.yml
  format: yaml
  label: Newscred Users API
  slug: newscred-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/openapi/newscred-users-api-openapi.yml
- filename: newscred-work-requests-api-openapi.yml
  format: yaml
  label: Newscred Work Requests API
  slug: newscred-work-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/openapi/newscred-work-requests-api-openapi.yml
- filename: newscred-workflows-api-openapi.yml
  format: yaml
  label: Newscred Workflows API
  slug: newscred-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/openapi/newscred-workflows-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Newscred Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Newscred secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Newscred
provider_slug: newscred
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.cmp.optimizely.com/o/oauth2/v1/auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://accounts.cmp.optimizely.com/o/oauth2/v1/token
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://accounts.cmp.optimizely.com/o/oauth2/v1/token
  name: OAuth2
  sources:
  - openapi/newscred-cmp-open-api-openapi.json
  type: oauth2
slug: newscred-authentication
source_filename: newscred-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://docs.developers.optimizely.com/content-marketing-platform/docs/authentication-1\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.cmp.optimizely.com/o/oauth2/v1/auth\n    tokenUrl: https://accounts.cmp.optimizely.com/o/oauth2/v1/token\n    scopes: 3\n  - flow: clientCredentials\n    tokenUrl: https://accounts.cmp.optimizely.com/o/oauth2/v1/token\n    scopes: 0\n  sources:\n  - openapi/newscred-cmp-open-api-openapi.json\ndocs: https://docs.developers.optimizely.com/content-marketing-platform/docs/authentication-1\nderived_from: openapi/newscred-cmp-open-api-openapi.json\nauthorization_server:\n  host: https://accounts.cmp.optimizely.com\n  authorization_endpoint: https://accounts.cmp.optimizely.com/o/oauth2/v1/auth\n  token_endpoint: https://accounts.cmp.optimizely.com/o/oauth2/v1/token\n\
  \  userinfo_endpoint: https://accounts.cmp.optimizely.com/o/oauth2/v1/userinfo\n  revocation: https://docs.developers.optimizely.com/content-marketing-platform/docs/revoke-tokens\n  legacy_host: https://accounts.welcomesoftware.com (Welcome-era; the legacy spec documents the same paths under\n    this host)\n  discovery: NONE — /.well-known/openid-configuration and /.well-known/oauth-authorization-server both return 404\n    on accounts.cmp.optimizely.com and accounts.welcomesoftware.com. An OAuth/OIDC client must be configured from\n    prose.\napp_registration:\n  self_serve: false\n  where: 'In-product only: Admin > Apps and Webhooks > Register App, inside an existing CMP organization.'\n  inputs:\n  - Mode (Production or Development)\n  - Name\n  - Description\n  - Expose Email Addresses?\n  - Homepage URL\n  - Authorization Callback URL\n  issues:\n  - client_id\n  - client_secret\n  note: There is no developer signup, no self-serve key issuance, and no public sandbox. API access\
  \ requires an\n    existing CMP tenancy.\ntoken_handling:\n  access_token: opaque UUID-shaped bearer token\n  refresh: refresh_token grant at the token endpoint; the @welcomesoftware/cmp-sdk documents automatic retry with\n    token refresh on authorization errors\n  revocation_docs: https://docs.developers.optimizely.com/content-marketing-platform/docs/revoke-tokens\nrfc_citations:\n- RFC 6749 s4.1 authorization code\n- RFC 6749 s4.4 client credentials\nlegacy_note: The legacy Welcome Open API spec documents the identical flow against https://accounts.welcomesoftware.com\n  with the same three scopes, and supported ONLY the authorization code flow. Client credentials is an Optimizely-era\n  addition.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/authentication/newscred-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Content Marketing
- Content Management
- Digital Asset Management
- Marketing
- Marketing Resource Management
- Workflows
- Publishing
- Webhook
- Acquired
---
