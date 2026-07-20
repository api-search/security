---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Lifesize Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lifesize secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lifesize
provider_slug: lifesize
scheme_count: 1
schemes:
- applies_to:
  - Lifesize Icon Automation API (REST)
  - Lifesize Automation Command Line Interface (CLI)
  credential_rotation_docs: https://support.lifesize.com/product/lifesize-icon-400-450-600-800/lets-get-started/system-access-and-passwords/
  default_credentials_documented: true
  description: Access to the Lifesize Icon automation API uses the same authentication policy as browser access to the system. Sign in to the Lifesize video system through an SSH or HTTP connection over the network with administrator credentials. The documented default username and password are "admin"; Lifesize documents changing system passwords as part of first-run configuration.
  name: adminCredentials
  scheme: basic
  sources:
  - https://support.lifesize.com/product/lifesize-icon-400-450-600-800/advanced-topics/api-overview/
  type: http
slug: lifesize-authentication
source_filename: lifesize-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://support.lifesize.com/product/lifesize-icon-400-450-600-800/advanced-topics/api-overview/\ndocs: https://support.lifesize.com/product/lifesize-icon-400-450-600-800/advanced-topics/api-overview/\nnotes: >-\n  Lifesize publishes no OpenAPI or Swagger definition, so this profile is captured\n  from the Lifesize Icon API overview documentation rather than derived from\n  securitySchemes. Lifesize was acquired by Enghouse Systems in 2023; the developer\n  documentation remains hosted on support.lifesize.com.\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  transport:\n  - https\n  - ssh\nschemes:\n- name: adminCredentials\n  type: http\n  scheme: basic\n  description: >-\n    Access to the Lifesize Icon automation API uses the same authentication policy as\n    browser access to the system. Sign in to the Lifesize video system through an SSH\n    or HTTP connection over the network with administrator\
  \ credentials. The documented\n    default username and password are \"admin\"; Lifesize documents changing system\n    passwords as part of first-run configuration.\n  sources:\n  - https://support.lifesize.com/product/lifesize-icon-400-450-600-800/advanced-topics/api-overview/\n  applies_to:\n  - Lifesize Icon Automation API (REST)\n  - Lifesize Automation Command Line Interface (CLI)\n  default_credentials_documented: true\n  credential_rotation_docs: https://support.lifesize.com/product/lifesize-icon-400-450-600-800/lets-get-started/system-access-and-passwords/\naccount_level_identity:\n  sso:\n    supported: true\n    scope: Lifesize Admin Console (account sign-in, not API authentication)\n    providers:\n    - Microsoft Azure AD\n    docs: https://support.lifesize.com/product/lifesize-admin-console/account-settings/sso-configuration/configure-using-microsoft-azure/\nnot_found:\n- oauth2 authorization server or documented scopes\n- published API keys or token issuance for the Lifesize\
  \ Cloud API\n- /.well-known/openid-configuration or /.well-known/oauth-authorization-server on any\n  Lifesize host (all probed hosts returned 403 or 404 on 2026-07-19)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lifesize/refs/heads/main/authentication/lifesize-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Video Conferencing
- Communications
- Collaboration
- Meetings
- Unified Communications
- Video
- Contact Center
- Conference Room Systems
- Streaming
---
