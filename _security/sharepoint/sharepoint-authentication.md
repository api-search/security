---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sharepoint-admin-edge-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Admin.edge API
  slug: sharepoint-admin-edge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-admin-edge-api-openapi.yml
- filename: sharepoint-groups-group-functions-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Groups.group.Functions API
  slug: sharepoint-groups-group-functions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-groups-group-functions-api-openapi.yml
- filename: sharepoint-groups-site-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Groups.site API
  slug: sharepoint-groups-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-groups-site-api-openapi.yml
- filename: sharepoint-sites-baseitem-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.base Item API
  slug: sharepoint-sites-baseitem-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-baseitem-api-openapi.yml
- filename: sharepoint-sites-basesitepage-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.base Site Page API
  slug: sharepoint-sites-basesitepage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-basesitepage-api-openapi.yml
- filename: sharepoint-sites-columndefinition-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.column Definition API
  slug: sharepoint-sites-columndefinition-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-columndefinition-api-openapi.yml
- filename: sharepoint-sites-contenttype-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.content Type API
  slug: sharepoint-sites-contenttype-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-contenttype-api-openapi.yml
- filename: sharepoint-sites-drive-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.drive API
  slug: sharepoint-sites-drive-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-drive-api-openapi.yml
- filename: sharepoint-sites-itemanalytics-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.item Analytics API
  slug: sharepoint-sites-itemanalytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-itemanalytics-api-openapi.yml
- filename: sharepoint-sites-list-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.list API
  slug: sharepoint-sites-list-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-list-api-openapi.yml
- filename: sharepoint-sites-onenote-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.onenote API
  slug: sharepoint-sites-onenote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-onenote-api-openapi.yml
- filename: sharepoint-sites-permission-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.permission API
  slug: sharepoint-sites-permission-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-permission-api-openapi.yml
- filename: sharepoint-sites-richlongrunningoperation-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.rich Long Running Operation API
  slug: sharepoint-sites-richlongrunningoperation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-richlongrunningoperation-api-openapi.yml
- filename: sharepoint-sites-site-actions-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.site.Actions API
  slug: sharepoint-sites-site-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-site-actions-api-openapi.yml
- filename: sharepoint-sites-site-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.site API
  slug: sharepoint-sites-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-site-api-openapi.yml
- filename: sharepoint-sites-site-functions-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.site.Functions API
  slug: sharepoint-sites-site-functions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-site-functions-api-openapi.yml
- filename: sharepoint-sites-store-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.store API
  slug: sharepoint-sites-store-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-store-api-openapi.yml
- filename: sharepoint-sites-user-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites.user API
  slug: sharepoint-sites-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-user-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Microsoft SharePoint Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Microsoft SharePoint secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Microsoft SharePoint
provider_slug: sharepoint
scheme_count: 1
schemes:
- description: OAuth 2.0 via Azure AD / Microsoft Identity Platform.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/sharepoint-rest-api.yaml
  type: oauth2
slug: sharepoint-authentication
source_filename: sharepoint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/sharepoint-rest-api.yaml\ndocs: https://learn.microsoft.com/en-us/graph/auth/\ndocs_sharepoint_rest: https://learn.microsoft.com/en-us/sharepoint/dev/sp-add-ins/authorization-and-authentication-of-sharepoint-add-ins\nnotes: >-\n  Both the SharePoint REST API and Microsoft Graph authenticate with OAuth 2.0 through\n  Microsoft Entra (Azure AD / Microsoft identity platform). Supports authorization code\n  (delegated), client credentials (app-only), and on-behalf-of flows. Tokens are bearer\n  tokens issued by login.microsoftonline.com. Write operations against the SharePoint REST\n  service additionally require the X-RequestDigest form-digest header.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n\
  \    scopes: 4\n  description: OAuth 2.0 via Azure AD / Microsoft Identity Platform.\n  sources:\n  - openapi/sharepoint-rest-api.yaml\n"
source_yaml_url: https://artifacts.apis.io/sharepoint/authentication/sharepoint-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Collaboration
- Document Management
- Enterprise Content Management
- Intranet
- Microsoft
---
