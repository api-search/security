---
anonymous_access: false
api_key_in: []
api_specs:
- filename: workday-business-processes-business-process-openapi.yml
  format: yaml
  label: Workday Business Processes Approvals API
  slug: workday-business-processes-approvals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-business-processes/refs/heads/main/openapi/workday-business-processes-business-process-openapi.yml
- filename: workday-business-processes-business-process-openapi.yml
  format: yaml
  label: Workday Business Processes Business Process Definitions API
  slug: workday-business-processes-business-process-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-business-processes/refs/heads/main/openapi/workday-business-processes-business-process-openapi.yml
- filename: workday-business-processes-business-process-openapi.yml
  format: yaml
  label: Workday Business Processes Inbox Items API
  slug: workday-business-processes-inbox-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-business-processes/refs/heads/main/openapi/workday-business-processes-business-process-openapi.yml
- filename: workday-business-processes-business-process-openapi.yml
  format: yaml
  label: Workday Business Processes Process Instances API
  slug: workday-business-processes-process-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-business-processes/refs/heads/main/openapi/workday-business-processes-business-process-openapi.yml
- filename: workday-business-processes-custom-business-process-config-openapi.yml
  format: yaml
  label: Workday Custom Business Process Config API
  slug: workday-business-processes-custom-business-process-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-business-processes/refs/heads/main/openapi/workday-business-processes-custom-business-process-config-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Workday Business Processes Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Workday Business Processes secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Workday Business Processes
provider_slug: workday-business-processes
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://{tenantAuthorizationHostname}/authorize
    flow: implicit
    scopes: 0
  name: OAuth2
  sources:
  - openapi/workday-business-processes-business-process-openapi.yml
  - openapi/workday-business-processes-custom-business-process-config-openapi.yml
  type: oauth2
slug: workday-business-processes-authentication
source_filename: workday-business-processes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: openapi/workday-business-processes-business-process-openapi.yml, openapi/workday-business-processes-custom-business-process-config-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\n  documented_flows:\n  - authorizationCode\n  - clientCredentials\n  - refreshToken\n  gateway: Workday Cloud Platform API Gateway — every REST call authenticates and routes through it\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://{tenantAuthorizationHostname}/authorize\n    scopes: 0\n  sources:\n  - openapi/workday-business-processes-business-process-openapi.yml\n  - openapi/workday-business-processes-custom-business-process-config-openapi.yml\ndocs: https://developer.workday.com/doc/GUID-6c598444-ce67-40d5-bd95-267ecfe439b8-enHYPHENus.md\ndocs_additional:\n- title: Create Your API Client\n  url: https://developer.workday.com/doc/zwx1518028675482.md\n- title: 'Reference:\
  \ OAuth2 Authorization Code'\n  url: https://developer.workday.com/doc/jzx1537909761291.md\n- title: 'Reference: OAuth2 Client Credentials'\n  url: https://developer.workday.com/doc/axp1537909839739.md\n- title: Request a New Access Token with a Refresh Token\n  url: https://developer.workday.com/doc/cqa1553122177664.md\n- title: SOAP API Authentication and Security\n  url: https://developer.workday.com/doc/GUID-4c354bdb-06cd-461d-a632-ea8303beaedb-enHYPHENus.md\nnotes: The published specs declare only an implicit flow, which is NOT what Workday tells integrators to use. The docs document\n  Authorization Code and Client Credentials as the supported flows for a registered API client, plus refresh-token renewal. Registration\n  is per tenant in the Developer Site Console and a client must be separately allowlisted onto each non-development tenant by a\n  Company Administrator. The SOAP side (wsdl/) authenticates differently again — WS-Security UsernameToken or X.509, with an Integration\n\
  \  System User, not OAuth. There is no OIDC discovery document and no RFC 8414 metadata on any Workday host (84 well-known probes\n  on 2026-09-17, all 404), so a client cannot discover the endpoints programmatically; they are tenant-specific and read from the\n  docs or the Console.\nsoap_auth:\n  mechanisms:\n  - WS-Security UsernameToken\n  - X.509 certificate\n  principal: Integration System User (ISU)\n  docs: https://developer.workday.com/doc/GUID-4c354bdb-06cd-461d-a632-ea8303beaedb-enHYPHENus.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-business-processes/refs/heads/main/authentication/workday-business-processes-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Business Processes
- Workflows
- Approvals
- Human Resources
- Enterprise
- Software-as-a-Service
- HCM
- Financial Management
- Process Automation
- Event Steps
- SOAP
- GraphQL
---
