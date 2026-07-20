---
api_key_in: []
auth_types:
- http
- oauth2
- cookie
description: ''
kind: authentication
layout: security
method: searched
name: Creatio Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Creatio secures its APIs with http, oauth2, and cookie across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Creatio
provider_slug: creatio
scheme_count: 4
schemes:
- cookies:
  - .ASPXAUTH
  - BPMLOADER
  - BPMCSRF
  - UserName
  description: 'Cookie-based forms authentication via the AuthService.svc web service. POST credentials to /ServiceModel/AuthService.svc/Login, then send the returned cookies (.ASPXAUTH, BPMLOADER, BPMCSRF, UserName) on subsequent requests. The BPMCSRF cookie value must also be echoed in the BPMCSRF request header, and requests set the ForceUseSession: true header.'
  endpoints:
    login: /ServiceModel/AuthService.svc/Login
  headers:
  - BPMCSRF
  - ForceUseSession
  name: forms-cookie
  recommended: true
  scheme: forms-authentication
  source: https://academy.creatio.com/docs/developer/integrations_and_api/authentication/authentication_basics/overview
  type: cookie
- description: OAuth 2.0 authorization for integrated applications. An OAuth client (client id + client secret) is registered in Creatio's Identity Service, which issues bearer access tokens presented on API requests. Grant type is client credentials (server-to-server). The token endpoint lives on the Identity Service configured for the instance.
  docs: https://academy.creatio.com/documents?id=2396
  name: oauth2
  scheme: clientCredentials
  source: https://academy.creatio.com/docs/developer/integrations_and_api/authentication/authentication_basics/overview
  type: oauth2
- description: HTTP Basic authentication is supported as an available authentication type.
  name: basic
  scheme: basic
  source: https://academy.creatio.com/docs/developer/integrations_and_api/authentication/authentication_basics/overview
  type: http
- description: Anonymous access is supported for web services explicitly configured to allow it.
  name: anonymous
  scheme: anonymous
  source: https://academy.creatio.com/docs/developer/integrations_and_api/authentication/authentication_basics/overview
  type: none
slug: creatio-authentication
source_filename: creatio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://academy.creatio.com/docs/developer/integrations_and_api/authentication/authentication_basics/overview\ndocs: https://academy.creatio.com/docs/developer/integrations_and_api/authentication/authentication_basics/overview\nsummary:\n  types: [http, oauth2, cookie]\n  api_key_in: []\n  oauth2_flows: [clientCredentials]\n  recommended: forms-cookie\n  notes: >-\n    Creatio is a multi-tenant platform; the API host is per instance\n    (https://<instance>.creatio.com). All external requests to OData and\n    DataService require authentication. Forms (cookie) authentication is the\n    recommended method for service-to-service integration; OAuth 2.0 is the\n    recommended method for integrated applications.\nschemes:\n  - name: forms-cookie\n    type: cookie\n    scheme: forms-authentication\n    description: >-\n      Cookie-based forms authentication via the AuthService.svc web service.\n      POST credentials to /ServiceModel/AuthService.svc/Login,\
  \ then send the\n      returned cookies (.ASPXAUTH, BPMLOADER, BPMCSRF, UserName) on subsequent\n      requests. The BPMCSRF cookie value must also be echoed in the BPMCSRF\n      request header, and requests set the ForceUseSession: true header.\n    endpoints:\n      login: /ServiceModel/AuthService.svc/Login\n    headers: [BPMCSRF, ForceUseSession]\n    cookies: ['.ASPXAUTH', BPMLOADER, BPMCSRF, UserName]\n    recommended: true\n    source: https://academy.creatio.com/docs/developer/integrations_and_api/authentication/authentication_basics/overview\n  - name: oauth2\n    type: oauth2\n    scheme: clientCredentials\n    description: >-\n      OAuth 2.0 authorization for integrated applications. An OAuth client\n      (client id + client secret) is registered in Creatio's Identity Service,\n      which issues bearer access tokens presented on API requests. Grant type\n      is client credentials (server-to-server). The token endpoint lives on the\n      Identity Service configured for\
  \ the instance.\n    docs: https://academy.creatio.com/documents?id=2396\n    source: https://academy.creatio.com/docs/developer/integrations_and_api/authentication/authentication_basics/overview\n  - name: basic\n    type: http\n    scheme: basic\n    description: HTTP Basic authentication is supported as an available authentication type.\n    source: https://academy.creatio.com/docs/developer/integrations_and_api/authentication/authentication_basics/overview\n  - name: anonymous\n    type: none\n    scheme: anonymous\n    description: Anonymous access is supported for web services explicitly configured to allow it.\n    source: https://academy.creatio.com/docs/developer/integrations_and_api/authentication/authentication_basics/overview\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creatio/refs/heads/main/authentication/creatio-authentication.yml
summary_line: http/oauth2/cookie · 4 schemes
tags:
- Company
- Saas
- CRM
- No-Code
- Low-Code
- Business Process Management
- Workflow Automation
- Sales
- Marketing
- Customer Service
- OData
- AI Agents
---
