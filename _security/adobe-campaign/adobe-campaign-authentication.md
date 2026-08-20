---
api_key_in:
- header
- cookie
api_specs:
- filename: adobe-campaign-custom-resources-api-openapi.yml
  format: yaml
  label: Adobe Campaign Custom Resources API
  slug: adobe-campaign-custom-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-custom-resources-api-openapi.yml
- filename: adobe-campaign-data-management-api-openapi.yml
  format: yaml
  label: Adobe Campaign Data Management API
  slug: adobe-campaign-data-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-data-management-api-openapi.yml
- filename: adobe-campaign-delivery-api-openapi.yml
  format: yaml
  label: Adobe Campaign Delivery API
  slug: adobe-campaign-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-delivery-api-openapi.yml
- filename: adobe-campaign-marketing-history-api-openapi.yml
  format: yaml
  label: Adobe Campaign Marketing History API
  slug: adobe-campaign-marketing-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-marketing-history-api-openapi.yml
- filename: adobe-campaign-metadata-api-openapi.yml
  format: yaml
  label: Adobe Campaign Metadata API
  slug: adobe-campaign-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-metadata-api-openapi.yml
- filename: adobe-campaign-organizational-units-api-openapi.yml
  format: yaml
  label: Adobe Campaign Organizational Units API
  slug: adobe-campaign-organizational-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-organizational-units-api-openapi.yml
- filename: adobe-campaign-privacy-api-openapi.yml
  format: yaml
  label: Adobe Campaign Privacy API
  slug: adobe-campaign-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-privacy-api-openapi.yml
- filename: adobe-campaign-profileandservices-api-openapi.yml
  format: yaml
  label: Adobe Campaign ProfileAndServices API
  slug: adobe-campaign-profileandservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-profileandservices-api-openapi.yml
- filename: adobe-campaign-profiles-api-openapi.yml
  format: yaml
  label: Adobe Campaign Profiles API
  slug: adobe-campaign-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-profiles-api-openapi.yml
- filename: adobe-campaign-query-definition-api-openapi.yml
  format: yaml
  label: Adobe Campaign Query Definition API
  slug: adobe-campaign-query-definition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-query-definition-api-openapi.yml
- filename: adobe-campaign-real-time-events-api-openapi.yml
  format: yaml
  label: Adobe Campaign Real-Time Events API
  slug: adobe-campaign-real-time-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-real-time-events-api-openapi.yml
- filename: adobe-campaign-session-management-api-openapi.yml
  format: yaml
  label: Adobe Campaign Session Management API
  slug: adobe-campaign-session-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-session-management-api-openapi.yml
- filename: adobe-campaign-subscription-api-openapi.yml
  format: yaml
  label: Adobe Campaign Subscription API
  slug: adobe-campaign-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-subscription-api-openapi.yml
- filename: adobe-campaign-subscriptions-api-openapi.yml
  format: yaml
  label: Adobe Campaign Subscriptions API
  slug: adobe-campaign-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-subscriptions-api-openapi.yml
- filename: adobe-campaign-transactional-messages-api-openapi.yml
  format: yaml
  label: Adobe Campaign Transactional Messages API
  slug: adobe-campaign-transactional-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-transactional-messages-api-openapi.yml
- filename: adobe-campaign-workflow-api-openapi.yml
  format: yaml
  label: Adobe Campaign Workflow API
  slug: adobe-campaign-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-workflow-api-openapi.yml
- filename: adobe-campaign-workflows-api-openapi.yml
  format: yaml
  label: Adobe Campaign Workflows API
  slug: adobe-campaign-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-workflows-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Adobe Campaign Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adobe Campaign secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Adobe Campaign
provider_slug: adobe-campaign
scheme_count: 3
schemes:
- authorization_endpoint: https://ims-na1.adobelogin.com/ims/authorize/v2
  bearerFormat: JWT
  description: Adobe IMS OAuth Server-to-Server access token. Obtained with a client_credentials exchange against https://ims-na1.adobelogin.com/ims/token/v3 using the Client ID and Client Secret issued by an Adobe Developer Console project that has the Adobe Campaign service added.
  docs: https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/implementation/
  issuer: https://ims-na1.adobelogin.com
  jwks_uri: https://ims-na1.adobelogin.com/ims/keys
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/_original/adobe-campaign-standard-openapi-original.yml
  - well-known/adobe-campaign-openid-configuration.json
  surface: Campaign Standard / Campaign v8 REST (https://mc.adobe.io/{ORGANIZATION}/campaign)
  token_endpoint: https://ims-na1.adobelogin.com/ims/token/v3
  type: http
- description: The Adobe Developer Console API Key (Client ID) for the integration. Sent on every REST call alongside the bearer token; a request with a valid bearer token but no X-Api-Key is rejected.
  docs: https://developer.adobe.com/developer-console/docs/guides/authentication/
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  required_with: BearerAuth
  sources:
  - openapi/_original/adobe-campaign-standard-openapi-original.yml
  - https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/apis/setting-up-api-access
  surface: Campaign Standard / Campaign v8 REST (https://mc.adobe.io/{ORGANIZATION}/campaign)
  type: apiKey
- description: Security token returned by xtk:session#Logon. Must be sent together with the __sessiontoken cookie on every authenticated Classic call. Tokens have a 24-hour lifecycle and are terminated with xtk:session#Logout.
  in: header
  name: SessionToken
  paired_with:
    in: cookie
    parameter: __sessiontoken
  parameter: X-Security-Token
  sources:
  - openapi/_original/adobe-campaign-classic-openapi-original.yml
  - openapi/adobe-campaign-session-management-api-openapi.yml
  - https://experienceleague.adobe.com/docs/campaign-classic/using/configuring-campaign-classic/api/web-service-calls.html
  surface: Campaign Classic SOAP-over-HTTP (https://{instance}.campaign.adobe.com)
  type: apiKey
slug: adobe-campaign-authentication
source_filename: adobe-campaign-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/apis/setting-up-api-access\n  and https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/apis/global-concepts/must-read\n  (fetched 2026-08-13); https://ims-na1.adobelogin.com/.well-known/openid-configuration\n  (probed 2026-08-13, HTTP 200); openapi/_original/adobe-campaign-classic-openapi-original.yml\n  and openapi/_original/adobe-campaign-standard-openapi-original.yml\nnotes: >-\n  Adobe Campaign has TWO distinct authentication models, one per deployment\n  surface, and they are not interchangeable. The REST surface on\n  https://mc.adobe.io/{ORGANIZATION}/campaign authenticates with an Adobe IMS\n  OAuth Server-to-Server access token in Authorization: Bearer PLUS an\n  X-Api-Key header carrying the Adobe Developer Console client ID — both are\n  required on every call. The Campaign Classic SOAP-over-HTTP surface on\n  https://{instance}.campaign.adobe.com\
  \ authenticates with a session token pair\n  obtained from xtk:session#Logon: the __sessiontoken cookie plus the\n  X-Security-Token header. Adobe's docs state Campaign APIs are server-to-server\n  only.\n  This file was regenerated by derive-authentication.py on 2026-08-13 against\n  the refined per-tag specs, which only carry the Classic SessionToken scheme;\n  the IMS bearer + API key schemes were restored from the _original specs and\n  upgraded against the live documentation, so this artifact is not weaker than\n  the round it replaced.\nsummary:\n  types:\n    - apiKey\n    - http\n    - oauth2\n  api_key_in:\n    - header\n    - cookie\n  server_to_server_only: true\nschemes:\n  - name: BearerAuth\n    surface: Campaign Standard / Campaign v8 REST (https://mc.adobe.io/{ORGANIZATION}/campaign)\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      Adobe IMS OAuth Server-to-Server access token. Obtained with a\n      client_credentials exchange against\n\
  \      https://ims-na1.adobelogin.com/ims/token/v3 using the Client ID and Client\n      Secret issued by an Adobe Developer Console project that has the Adobe\n      Campaign service added.\n    token_endpoint: https://ims-na1.adobelogin.com/ims/token/v3\n    authorization_endpoint: https://ims-na1.adobelogin.com/ims/authorize/v2\n    issuer: https://ims-na1.adobelogin.com\n    jwks_uri: https://ims-na1.adobelogin.com/ims/keys\n    docs: https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/implementation/\n    sources:\n      - openapi/_original/adobe-campaign-standard-openapi-original.yml\n      - well-known/adobe-campaign-openid-configuration.json\n  - name: ApiKeyAuth\n    surface: Campaign Standard / Campaign v8 REST (https://mc.adobe.io/{ORGANIZATION}/campaign)\n    type: apiKey\n    in: header\n    parameter: X-Api-Key\n    required_with: BearerAuth\n    description: >-\n      The Adobe Developer Console API Key (Client ID) for the\
  \ integration. Sent\n      on every REST call alongside the bearer token; a request with a valid\n      bearer token but no X-Api-Key is rejected.\n    docs: https://developer.adobe.com/developer-console/docs/guides/authentication/\n    sources:\n      - openapi/_original/adobe-campaign-standard-openapi-original.yml\n      - https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/apis/setting-up-api-access\n  - name: SessionToken\n    surface: Campaign Classic SOAP-over-HTTP (https://{instance}.campaign.adobe.com)\n    type: apiKey\n    in: header\n    parameter: X-Security-Token\n    description: >-\n      Security token returned by xtk:session#Logon. Must be sent together with\n      the __sessiontoken cookie on every authenticated Classic call. Tokens have\n      a 24-hour lifecycle and are terminated with xtk:session#Logout.\n    paired_with:\n      in: cookie\n      parameter: __sessiontoken\n    sources:\n      - openapi/_original/adobe-campaign-classic-openapi-original.yml\n\
  \      - openapi/adobe-campaign-session-management-api-openapi.yml\n      - https://experienceleague.adobe.com/docs/campaign-classic/using/configuring-campaign-classic/api/web-service-calls.html\ntenancy:\n  organization_id:\n    description: >-\n      Every REST path is scoped by an ORGANIZATION ID issued by Adobe per\n      instance. The production instance uses <ORGANIZATION>; the staging instance\n      uses <ORGANIZATION-mkt-stage>.\n    production_pattern: https://mc.adobe.io/<ORGANIZATION>/campaign\n    stage_pattern: https://mc.adobe.io/<ORGANIZATION-mkt-stage>/campaign\n  authorization_model: >-\n    Campaign APIs run in the administrator context by default and are excluded\n    from the role context — organizational units and roles do NOT apply to API\n    callers unless Adobe explicitly configures it. This is a meaningful blast-radius\n    fact for any agent integration.\ndeprecated:\n  - mechanism: Service Account (JWT) credential\n    replaced_by: OAuth Server-to-Server credential\n\
  \    end_of_support: '2025-01-27'\n    source: https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/apis/setting-up-api-access\n    note: >-\n      JWT service-account credentials stopped working 2025-01-27. Campaign v8.5.1\n      also made Adobe IMS mandatory for technical operators connecting to\n      Campaign.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/authentication/adobe-campaign-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
- Transactional Messaging
- Customer Data
- Adobe Experience Cloud
- SMS
- Push Notifications
- Workflow-Automation
- Privacy
---
