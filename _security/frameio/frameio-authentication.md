---
api_key_in: []
api_specs:
- filename: frameio-account-permissions-api-openapi.yml
  format: yaml
  label: Frame.io Account Permissions API
  slug: frameio-account-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/openapi/frameio-account-permissions-api-openapi.yml
- filename: frameio-accounts-api-openapi.yml
  format: yaml
  label: Frame.io Accounts API
  slug: frameio-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/openapi/frameio-accounts-api-openapi.yml
- filename: frameio-collections-api-openapi.yml
  format: yaml
  label: Frame.io Collections API
  slug: frameio-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/openapi/frameio-collections-api-openapi.yml
- filename: frameio-comments-api-openapi.yml
  format: yaml
  label: Frame.io Comments API
  slug: frameio-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/openapi/frameio-comments-api-openapi.yml
- filename: frameio-custom-actions-api-openapi.yml
  format: yaml
  label: Frame.io Custom Actions API
  slug: frameio-custom-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/openapi/frameio-custom-actions-api-openapi.yml
- filename: frameio-files-api-openapi.yml
  format: yaml
  label: Frame.io Files API
  slug: frameio-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/openapi/frameio-files-api-openapi.yml
- filename: frameio-folder-permissions-api-openapi.yml
  format: yaml
  label: Frame.io Folder Permissions API
  slug: frameio-folder-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/openapi/frameio-folder-permissions-api-openapi.yml
- filename: frameio-folders-api-openapi.yml
  format: yaml
  label: Frame.io Folders API
  slug: frameio-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/openapi/frameio-folders-api-openapi.yml
- filename: frameio-groups-api-openapi.yml
  format: yaml
  label: Frame.io Groups API
  slug: frameio-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/openapi/frameio-groups-api-openapi.yml
- filename: frameio-metadata-api-openapi.yml
  format: yaml
  label: Frame.io Metadata API
  slug: frameio-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/openapi/frameio-metadata-api-openapi.yml
- filename: frameio-metadata-fields-api-openapi.yml
  format: yaml
  label: Frame.io Metadata Fields API
  slug: frameio-metadata-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/openapi/frameio-metadata-fields-api-openapi.yml
- filename: frameio-project-permissions-api-openapi.yml
  format: yaml
  label: Frame.io Project Permissions API
  slug: frameio-project-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/openapi/frameio-project-permissions-api-openapi.yml
- filename: frameio-projects-api-openapi.yml
  format: yaml
  label: Frame.io Projects API
  slug: frameio-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/openapi/frameio-projects-api-openapi.yml
- filename: frameio-search-api-openapi.yml
  format: yaml
  label: Frame.io Search API
  slug: frameio-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/openapi/frameio-search-api-openapi.yml
- filename: frameio-shares-api-openapi.yml
  format: yaml
  label: Frame.io Shares API
  slug: frameio-shares-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/openapi/frameio-shares-api-openapi.yml
- filename: frameio-users-api-openapi.yml
  format: yaml
  label: Frame.io Users API
  slug: frameio-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/openapi/frameio-users-api-openapi.yml
- filename: frameio-version-stacks-api-openapi.yml
  format: yaml
  label: Frame.io Version Stacks API
  slug: frameio-version-stacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/openapi/frameio-version-stacks-api-openapi.yml
- filename: frameio-webhooks-api-openapi.yml
  format: yaml
  label: Frame.io Webhooks API
  slug: frameio-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/openapi/frameio-webhooks-api-openapi.yml
- filename: frameio-workspace-permissions-api-openapi.yml
  format: yaml
  label: Frame.io Workspace Permissions API
  slug: frameio-workspace-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/openapi/frameio-workspace-permissions-api-openapi.yml
- filename: frameio-workspaces-api-openapi.yml
  format: yaml
  label: Frame.io Workspaces API
  slug: frameio-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/openapi/frameio-workspaces-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Frameio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Frame.io secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Frame.io
provider_slug: frameio
scheme_count: 2
schemes:
- description: 'For more information, see: https://developer.adobe.com/frameio'
  flows:
  - authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3
  name: OAuth2
  sources:
  - openapi/frameio-v4-openapi.json
  type: oauth2
- description: Server to server authentication flow
  flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3
  name: s2s_auth
  sources:
  - openapi/frameio-v4-openapi.json
  type: oauth2
slug: frameio-authentication
source_filename: frameio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/frameio-v4-openapi.json\ndocs: https://next.developer.frame.io/platform/v4/docs/guides/authentication/overview\nnote: OAuth2 via Adobe IMS (ims-na1.adobelogin.com). authorizationCode flow for user\n  apps (Web/SPA/Native with PKCE), clientCredentials for server-to-server. Legacy\n  developer tokens supported via the x-frameio-legacy-token-auth header.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2\n    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3\n    scopes: 4\n  description: 'For more information, see: https://developer.adobe.com/frameio'\n  sources:\n  - openapi/frameio-v4-openapi.json\n- name: s2s_auth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3\n\
  \    scopes: 3\n  description: Server to server authentication flow\n  sources:\n  - openapi/frameio-v4-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/authentication/frameio-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Media
- Video
- Collaboration
- Review and Approval
- Media Production
- Adobe
- Content
---
