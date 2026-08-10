---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Clockworks Analytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clockworks Analytics secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Clockworks Analytics
provider_slug: clockworks-analytics
scheme_count: 2
schemes:
- applies_to:
  - https://rest.buildingsapi.net/core-base
  - https://rest.buildingsapi.net/core-diag
  - https://rest.buildingsapi.net/core-kpis
  in: header
  issuance: URL endpoint and subscription key are provisioned by Clockworks Analytics once the API subscriber is registered; keys are scoped to the buildings and equipment the associated user account may access.
  name: ApimSubscriptionKey
  parameter_name: Ocp-Apim-Subscription-Key
  sources:
  - https://cw.clockworksanalytics.com/APIDocumentation.aspx
  type: apiKey
  x-evidence:
    fetched: '2026-08-09'
    http_status: 401
    url: https://rest.buildingsapi.net/core-base/clients
    www_authenticate: AzureApiManagementKey realm="https://rest.buildingsapi.net/core-base",name="Ocp-Apim-Subscription-Key",type="header"
- applies_to:
  - https://rest.buildingsapi.net/workorders
  header: 'Authorization: {{bearerToken}}'
  name: WorkOrdersBearerToken
  scheme: bearer
  sources:
  - https://clockworksanalytics.atlassian.net/wiki/spaces/ClockworksAnalyticsUM/pages/5742297089/CMMS+Integration+Developer+Guide+version+2
  token_endpoint: https://rest.buildingsapi.net/workorders/auth/token
  token_endpoint_method: POST
  token_lifetime_seconds: 3599
  token_request_body:
  - clientId
  - clientSecret
  token_response_field: data.accessToken
  type: http
slug: clockworks-analytics-authentication
source_filename: clockworks-analytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://cw.clockworksanalytics.com/APIDocumentation.aspx\ndocs:\n- https://cw.clockworksanalytics.com/APIDocumentation.aspx\n- https://clockworksanalytics.atlassian.net/wiki/spaces/ClockworksAnalyticsUM/pages/5742297089/CMMS+Integration+Developer+Guide+version+2\nnote: >-\n  Clockworks publishes no OpenAPI, so this profile is read from the provider's own public\n  API documentation rather than derived from securitySchemes. The API is fronted by Azure\n  API Management and splits authentication by container: the read/asset containers use an\n  APIM subscription key, the work-order container uses a bearer token minted from a\n  clientId/clientSecret pair.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  containers_with_distinct_credentials: 2\nschemes:\n- name: ApimSubscriptionKey\n  type: apiKey\n  in: header\n  parameter_name: Ocp-Apim-Subscription-Key\n  applies_to:\n  - https://rest.buildingsapi.net/core-base\n\
  \  - https://rest.buildingsapi.net/core-diag\n  - https://rest.buildingsapi.net/core-kpis\n  issuance: >-\n    URL endpoint and subscription key are provisioned by Clockworks Analytics once the API\n    subscriber is registered; keys are scoped to the buildings and equipment the associated\n    user account may access.\n  sources:\n  - https://cw.clockworksanalytics.com/APIDocumentation.aspx\n  x-evidence:\n    fetched: '2026-08-09'\n    url: https://rest.buildingsapi.net/core-base/clients\n    http_status: 401\n    www_authenticate: AzureApiManagementKey realm=\"https://rest.buildingsapi.net/core-base\",name=\"Ocp-Apim-Subscription-Key\",type=\"header\"\n- name: WorkOrdersBearerToken\n  type: http\n  scheme: bearer\n  applies_to:\n  - https://rest.buildingsapi.net/workorders\n  token_endpoint: https://rest.buildingsapi.net/workorders/auth/token\n  token_endpoint_method: POST\n  token_request_body:\n  - clientId\n  - clientSecret\n  token_response_field: data.accessToken\n  token_lifetime_seconds:\
  \ 3599\n  header: 'Authorization: {{bearerToken}}'\n  sources:\n  - https://clockworksanalytics.atlassian.net/wiki/spaces/ClockworksAnalyticsUM/pages/5742297089/CMMS+Integration+Developer+Guide+version+2\nrequired_headers:\n- name: Accept\n  value: application/vnd.api+json\n- name: Content-Type\n  value: application/json\n- name: Ocp-Apim-Subscription-Key\n  value: '{Subscription Key}'\n  applies_to: base/diag/kpi containers\n- name: ApiVersion\n  value: '{API Version}'\n- name: ApiDocVersion\n  value: '{API Doc Version}'\n- name: APIVersion\n  value: '3.0'\n  applies_to: workorders auth/token request\nscopes_published: false\nscopes_note: >-\n  No OAuth 2.0 authorization server, no scope reference and no OpenID Connect discovery\n  document were found on any Clockworks host; access is scoped by the provisioned user\n  account behind the subscription key, not by declared scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clockworks-analytics/refs/heads/main/authentication/clockworks-analytics-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Building Analytics
- Fault Detection and Diagnostics
- HVAC
- Energy Management
- Facilities Management
- Smart Buildings
- CMMS Integration
- Analytics
- Internet of Things
---
