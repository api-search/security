---
anonymous_access: false
api_key_in: []
api_specs:
- filename: five9-open-messaging-api.postman_collection.json
  format: json
  label: Five9 Open Messaging API
  slug: open-messaging-api
  spec_type: Postman
  url: https://artifacts.apis.io/five9/openapi/_original/five9-open-messaging-api.postman_collection.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Five9 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Five9 declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Five9
provider_slug: five9
scheme_count: 4
schemes:
- applies_to: Five9 "New Platform APIs" (e.g. Open Messaging, messaging-service/v1)
  credentials: 'Client Secret credentials created in Admin Console API Access Control: "API access with customizable scopes for Five9 New Platform APIs . Each application can have up to two active credentials." Family and scopes are selected per credential; duration "Never Expires or Custom".'
  evidence:
  - https://documentation.five9.com/bundle/admin-console/page/admin-console/api-access-control/configuring-api-access-control.htm
  - https://github.com/Five9DeveloperProgram/openmessaging-api
  flow: clientCredentials
  id: oauth2-client-credentials
  note: API Access Control is documented as "under controlled availability (CA)".
  token_request: POST, grant_type=client_credentials, Authorization Basic of the secret:key pair (per the provider's Postman collection)
  token_url: '{baseUrl}/oauth2/v1/token'
  type: oauth2
- applies_to: Identity Services SCIM provisioning
  credentials: '"API Key : Specific to Identity Services SCIM integrations. Family and scopes are predefined and cannot be customized."'
  evidence:
  - https://documentation.five9.com/bundle/admin-console/page/admin-console/api-access-control/configuring-api-access-control.htm
  id: api-key-scim
  type: apiKey
- applies_to: Configuration Web Services (SOAP, api.five9.com/wsadmin/v13), Statistics Web Services, CloudAuth / NG REST
  credentials: Five9 user (or "API Only User") username and password
  evidence:
  - https://github.com/Five9DeveloperProgram/PSFive9Admin
  - https://github.com/Five9DeveloperProgram/PSFive9CloudAPI
  id: basic-username-password
  note: Stated in Five9DeveloperProgram sample READMEs ("The module uses basic authentication over HTTPS."), not on a public docs page; the developer guides are login-gated PDFs.
  scheme: basic
  type: http
- applies_to: VCC Agent and Supervisor REST APIs
  evidence:
  - https://github.com/Five9DeveloperProgram/Five9-Agent-Sup-REST-API-Starter-Kit
  id: session-rest
  note: The starter kit obtains session metadata from app.five9.com/appsvcs/rs/svc/auth/metadata; the developer guide itself requires a docs login. Not called.
  type: session
slug: five9-authentication
source_filename: five9-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: searched\nsource: https://documentation.five9.com/bundle/admin-console/page/admin-console/api-access-control/configuring-api-access-control.htm\ndocs: https://documentation.five9.com/bundle/admin-console/page/admin-console/api-access-control/api-access-control.htm\nname: Five9 authentication\nschemes:\n- id: oauth2-client-credentials\n  type: oauth2\n  flow: clientCredentials\n  applies_to: Five9 \"New Platform APIs\" (e.g. Open Messaging, messaging-service/v1)\n  token_url: '{baseUrl}/oauth2/v1/token'\n  token_request: POST, grant_type=client_credentials, Authorization Basic of the secret:key pair (per the provider's Postman collection)\n  credentials: >-\n    Client Secret credentials created in Admin Console API Access Control: \"API access with customizable scopes for\n    Five9 New Platform APIs . Each application can have up to two active credentials.\" Family and scopes are selected\n    per credential; duration \"Never Expires or Custom\"\
  .\n  evidence:\n  - https://documentation.five9.com/bundle/admin-console/page/admin-console/api-access-control/configuring-api-access-control.htm\n  - https://github.com/Five9DeveloperProgram/openmessaging-api\n  note: API Access Control is documented as \"under controlled availability (CA)\".\n- id: api-key-scim\n  type: apiKey\n  applies_to: Identity Services SCIM provisioning\n  credentials: '\"API Key : Specific to Identity Services SCIM integrations. Family and scopes are predefined and cannot be customized.\"'\n  evidence:\n  - https://documentation.five9.com/bundle/admin-console/page/admin-console/api-access-control/configuring-api-access-control.htm\n- id: basic-username-password\n  type: http\n  scheme: basic\n  applies_to: Configuration Web Services (SOAP, api.five9.com/wsadmin/v13), Statistics Web Services, CloudAuth / NG REST\n  credentials: Five9 user (or \"API Only User\") username and password\n  evidence:\n  - https://github.com/Five9DeveloperProgram/PSFive9Admin\n  - https://github.com/Five9DeveloperProgram/PSFive9CloudAPI\n\
  \  note: Stated in Five9DeveloperProgram sample READMEs (\"The module uses basic authentication over HTTPS.\"), not on a public docs page; the developer guides are login-gated PDFs.\n- id: session-rest\n  type: session\n  applies_to: VCC Agent and Supervisor REST APIs\n  evidence:\n  - https://github.com/Five9DeveloperProgram/Five9-Agent-Sup-REST-API-Starter-Kit\n  note: The starter kit obtains session metadata from app.five9.com/appsvcs/rs/svc/auth/metadata; the developer guide itself requires a docs login. Not called.\ncors: Browser integrations must allowlist their origin in VCC configuration (no wildcards) — https://documentation.five9.com/bundle/basic-admin/page/basic-admin/domain-settings/enabling-access-to-the-rest-api.htm\n"
source_yaml_url: https://artifacts.apis.io/five9/authentication/five9-authentication.yml
summary_line: 4 schemes
tags:
- Contact Center
- CCaaS
- Cloud Telephony
- Customer Engagement
- Omnichannel
- Workforce Optimization
- Virtual Agents
- Agent Assist
---
