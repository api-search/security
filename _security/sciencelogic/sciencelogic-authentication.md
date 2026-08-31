---
api_key_in:
- cookie
- header
api_specs:
- filename: sciencelogic-skylar-compliance-openapi.json
  format: json
  label: Skylar Compliance API
  slug: skylar-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sciencelogic/refs/heads/main/openapi/sciencelogic-skylar-compliance-openapi.json
auth_types:
- apiKey
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Sciencelogic Authentication
name_suffix: Authentication
oauth_flows: []
overview: ScienceLogic secures its APIs with apiKey and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ScienceLogic
provider_slug: sciencelogic
scheme_count: 3
schemes:
- description: 'The Skylar Compliance web interface uses session cookies to authenticate API requests coming from a user''s browser.

    Please use authentication tokens when integrating with the Skylar Compliance API programmatically.


    Example header:


    ```http

    Cookie: session=abcde12345; Path=/; HttpOnly

    ```'
  in: cookie
  name: Cookie
  parameter: session
  sources:
  - openapi/sciencelogic-skylar-compliance-openapi.json
  type: apiKey
- description: 'To integrate with the Skylar Compliance API, please use the web interface to create API tokens. API requests via

    token should pass an `Authorization` header using the `Custom` prefix.


    Example header:


    ```http

    Authorization: Custom qVUXmMhPsle3NVU...

    ```'
  in: header
  name: Token
  parameter: Authorization
  sources:
  - openapi/sciencelogic-skylar-compliance-openapi.json
  type: apiKey
- description: 'Lists required [Permissions](#tag/Permission) for each individual endpoint.


    **Please note:** Whilst this authentication method is listed as an OpenID Connect authentication type, it

    is only used for the purposes of displaying the required permissions on each endpoint and is _not_ a valid

    authentication method by itself.


    - `ModifyDevice`

    - `BackupDevice`

    - `RestoreDevice`

    - `CommandDevice`

    - `Vie'
  name: Permissions
  openIdConnectUrl: https://ignore.example.com
  sources:
  - openapi/sciencelogic-skylar-compliance-openapi.json
  type: openIdConnect
slug: sciencelogic-authentication
source_filename: sciencelogic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: derived\nsource: openapi/sciencelogic-skylar-compliance-openapi.json\nsummary:\n  types:\n  - apiKey\n  - openIdConnect\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: Cookie\n  type: apiKey\n  in: cookie\n  parameter: session\n  description: |-\n    The Skylar Compliance web interface uses session cookies to authenticate API requests coming from a user's browser.\n    Please use authentication tokens when integrating with the Skylar Compliance API programmatically.\n\n    Example header:\n\n    ```http\n    Cookie: session=abcde12345; Path=/; HttpOnly\n    ```\n  sources:\n  - openapi/sciencelogic-skylar-compliance-openapi.json\n- name: Token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    To integrate with the Skylar Compliance API, please use the web interface to create API tokens. API requests via\n    token should pass an `Authorization` header using the `Custom` prefix.\n\n    Example header:\n\
  \n    ```http\n    Authorization: Custom qVUXmMhPsle3NVU...\n    ```\n  sources:\n  - openapi/sciencelogic-skylar-compliance-openapi.json\n- name: Permissions\n  type: openIdConnect\n  openIdConnectUrl: https://ignore.example.com\n  description: |-\n    Lists required [Permissions](#tag/Permission) for each individual endpoint.\n\n    **Please note:** Whilst this authentication method is listed as an OpenID Connect authentication type, it\n    is only used for the purposes of displaying the required permissions on each endpoint and is _not_ a valid\n    authentication method by itself.\n\n    - `ModifyDevice`\n    - `BackupDevice`\n    - `RestoreDevice`\n    - `CommandDevice`\n    - `Vie\n  sources:\n  - openapi/sciencelogic-skylar-compliance-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sciencelogic/refs/heads/main/authentication/sciencelogic-authentication.yml
summary_line: apiKey/openIdConnect · 3 schemes
tags:
- AIOps
- IT Operations
- Observability
- Monitoring
- Network Configuration Management
- Compliance
- Automation
- Incident Management
---
