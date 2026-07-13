---
api_key_in: []
api_specs:
- filename: radius-applications-core-openapi.json
  format: json
  label: Radius Applications.Core API
  slug: applications-core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radius/refs/heads/main/openapi/radius-applications-core-openapi.json
- filename: radius-applications-dapr-openapi.json
  format: json
  label: Radius Applications.Dapr API
  slug: applications-dapr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radius/refs/heads/main/openapi/radius-applications-dapr-openapi.json
- filename: radius-applications-datastores-openapi.json
  format: json
  label: Radius Applications.Datastores API
  slug: applications-datastores
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radius/refs/heads/main/openapi/radius-applications-datastores-openapi.json
- filename: radius-applications-messaging-openapi.json
  format: json
  label: Radius Applications.Messaging API
  slug: applications-messaging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radius/refs/heads/main/openapi/radius-applications-messaging-openapi.json
- filename: radius-ucp-openapi.json
  format: json
  label: Radius Universal Control Plane (UCP) API
  slug: ucp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radius/refs/heads/main/openapi/radius-ucp-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Radius Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Radius secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Radius
provider_slug: radius
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/radius-applications-core-openapi.json
  - openapi/radius-applications-dapr-openapi.json
  - openapi/radius-applications-datastores-openapi.json
  - openapi/radius-applications-messaging-openapi.json
  - openapi/radius-ucp-openapi.json
  type: oauth2
slug: radius-authentication
source_filename: radius-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/radius-applications-core-openapi.json, openapi/radius-applications-dapr-openapi.json,\n  openapi/radius-applications-datastores-openapi.json, openapi/radius-applications-messaging-openapi.json,\n  openapi/radius-ucp-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow.\n  sources:\n  - openapi/radius-applications-core-openapi.json\n  - openapi/radius-applications-dapr-openapi.json\n  - openapi/radius-applications-datastores-openapi.json\n  - openapi/radius-applications-messaging-openapi.json\n  - openapi/radius-ucp-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/radius/refs/heads/main/authentication/radius-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Application Platform
- Cloud Native
- Infrastructure
- Multi Cloud
---
