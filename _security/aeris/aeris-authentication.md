---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: aeris-auth-3.0-openapi.yaml
  format: yaml
  label: Aeris IoT Accelerator REST API
  slug: aeris-iot-accelerator-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeris/refs/heads/main/openapi/aeris-auth-3.0-openapi.yaml
- filename: aeris-sms-messaging-api-openapi.yaml
  format: yaml
  label: Aeris IoT Accelerator SMS Messaging API
  slug: aeris-iot-accelerator-sms-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeris/refs/heads/main/openapi/aeris-sms-messaging-api-openapi.yaml
- filename: aeris-watchtower-api-openapi-openapi.yaml
  format: yaml
  label: Aeris IoT Watchtower API
  slug: aeris-iot-watchtower-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeris/refs/heads/main/openapi/aeris-watchtower-api-openapi-openapi.yaml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Aeris Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- password
overview: Aeris secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and password flow(s).
provider_name: Aeris
provider_slug: aeris
scheme_count: 5
schemes:
- flows:
  - flow: password
    scopes: 17
    tokenUrl: /iot/api/auth/token
  name: Oauth2_auth
  sources:
  - openapi/aeris-business-analytics-report-api-openapi.yaml
  - openapi/aeris-business-automation-api-openapi.yaml
  - openapi/aeris-consumer-connectivity-openapi.yaml
  - openapi/aeris-enterprise-management-api-openapi.yaml
  - openapi/aeris-incidents-external-api-openapi.yaml
  - openapi/aeris-operator-order-management-api-openapi.yaml
  - openapi/aeris-organization-signaling-aggregations-api-openapi.yaml
  - openapi/aeris-resource-inventory-api-openapi.yaml
  - openapi/aeris-shared-bundle-api-openapi.yaml
  - openapi/aeris-sim-specification-management-api-openapi.yaml
  - openapi/aeris-subscription-change-history-openapi.yaml
  - openapi/aeris-subscription-custom-fields-api-openapi.yaml
  - openapi/aeris-subscription-device-api-openapi.yaml
  - openapi/aeris-subscription-device-reconnect-api-openapi.yaml
  - openapi/aeris-subscription-inventory-common-api-openapi.yaml
  - openapi/aeris-subscription-location-api-openapi.yaml
  - openapi/aeris-subscription-number-management-api-openapi.yaml
  - openapi/aeris-subscription-search-api-openapi.yaml
  - openapi/aeris-subscription-signalling-events-api-openapi.yaml
  - openapi/aeris-subscription-signalling-usages-api-openapi.yaml
  type: oauth2
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/aeris-business-automation-api-openapi.yaml
  type: http
- description: The resources in the API are protected using the OAuth 2.0 protocol
  flows:
  - flow: clientCredentials
    scopes: 4
    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token
  name: OAuth2
  sources:
  - openapi/aeris-eco-operations-api-openapi.yaml
  - openapi/aeris-eim-info-api-openapi.yaml
  - openapi/aeris-euicc-setup-api-openapi.yaml
  - openapi/aeris-watchtower-api-openapi-openapi.yaml
  type: oauth2
- description: Input token directly or use login endpoints
  in: header
  name: token
  parameter: X-Access-Token
  sources:
  - openapi/aeris-mds-esb-device-localization-openapi.yaml
  - openapi/aeris-mds-esb-subscription-management-openapi.yaml
  type: apiKey
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/aeris-sms-messaging-api-openapi.yaml
  type: http
slug: aeris-authentication
source_filename: aeris-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: searched\nsource: openapi/aeris-business-analytics-report-api-openapi.yaml, openapi/aeris-business-automation-api-openapi.yaml,\n  openapi/aeris-consumer-connectivity-openapi.yaml, openapi/aeris-eco-operations-api-openapi.yaml, openapi/aeris-eim-info-api-openapi.yaml,\n  openapi/aeris-enterprise-management-api-openapi.yaml, openapi/aeris-euicc-setup-api-openapi.yaml, openapi/aeris-incidents-external-api-openapi.yaml,\n  openapi/aeris-mds-esb-device-localization-openapi.yaml, openapi/aeris-mds-esb-subscription-management-openapi.yaml,\n  openapi/aeris-operator-order-management-api-openapi.yaml, openapi/aeris-organization-signaling-aggregations-api-openapi.yaml\n  ... — upgraded from the Aeris IoT Developer Portal API Quick start guide, which publishes the authentication mechanism\n  used by each API group.\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  - password\nschemes:\n\
  - name: Oauth2_auth\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: /iot/api/auth/token\n    scopes: 17\n  sources:\n  - openapi/aeris-business-analytics-report-api-openapi.yaml\n  - openapi/aeris-business-automation-api-openapi.yaml\n  - openapi/aeris-consumer-connectivity-openapi.yaml\n  - openapi/aeris-enterprise-management-api-openapi.yaml\n  - openapi/aeris-incidents-external-api-openapi.yaml\n  - openapi/aeris-operator-order-management-api-openapi.yaml\n  - openapi/aeris-organization-signaling-aggregations-api-openapi.yaml\n  - openapi/aeris-resource-inventory-api-openapi.yaml\n  - openapi/aeris-shared-bundle-api-openapi.yaml\n  - openapi/aeris-sim-specification-management-api-openapi.yaml\n  - openapi/aeris-subscription-change-history-openapi.yaml\n  - openapi/aeris-subscription-custom-fields-api-openapi.yaml\n  - openapi/aeris-subscription-device-api-openapi.yaml\n  - openapi/aeris-subscription-device-reconnect-api-openapi.yaml\n  - openapi/aeris-subscription-inventory-common-api-openapi.yaml\n\
  \  - openapi/aeris-subscription-location-api-openapi.yaml\n  - openapi/aeris-subscription-number-management-api-openapi.yaml\n  - openapi/aeris-subscription-search-api-openapi.yaml\n  - openapi/aeris-subscription-signalling-events-api-openapi.yaml\n  - openapi/aeris-subscription-signalling-usages-api-openapi.yaml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/aeris-business-automation-api-openapi.yaml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token\n    scopes: 4\n  description: The resources in the API are protected using the OAuth 2.0 protocol\n  sources:\n  - openapi/aeris-eco-operations-api-openapi.yaml\n  - openapi/aeris-eim-info-api-openapi.yaml\n  - openapi/aeris-euicc-setup-api-openapi.yaml\n  - openapi/aeris-watchtower-api-openapi-openapi.yaml\n- name: token\n  type: apiKey\n  in: header\n  parameter: X-Access-Token\n  description: Input token directly\
  \ or use login endpoints\n  sources:\n  - openapi/aeris-mds-esb-device-localization-openapi.yaml\n  - openapi/aeris-mds-esb-subscription-management-openapi.yaml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/aeris-sms-messaging-api-openapi.yaml\ndocs:\n- https://iotdeveloper.aeris.net/hc/en-us/articles/25348523998748-API-Quick-start-guide\n- https://iotdeveloper.aeris.net/hc/en-us/articles/25348574275868-JWT-Authentication-Best-Practices\n- https://iotdeveloper.aeris.net/hc/en-us/articles/25348572926236-Auth-API-1-0-1\ndocs_findings:\n  token_endpoints:\n    bearer: POST /iot/api/auth and POST /iot/api/auth/token\n    x_access_token: POST /login (per API group)\n    marketplace_hub: POST /auth/login\n  by_api_group:\n    Service Portal (SOAP): wss-security UsernameToken\n    User Administration: X-access-token via POST /login\n    Consumer Connectivity: X-access-token via POST /login\n    Subscription Management: X-access-token via POST /login\n    Device Localization:\
  \ X-access-token via POST /login\n    Shared bundle: Bearer via POST /token\n    Enterprise Management (CSP only): Bearer via POST /token\n    eUICC Setup (CSP and Advanced Resellers only): Bearer via POST /token\n    Device Reconnect: Bearer via POST /token\n    Subscription Change History: Bearer via POST /token\n    Subscription management - additional functions: Bearer via POST /token\n    Search Subscription Details: Bearer via POST /token\n    Ticketing service for incident management: Bearer via POST /token\n    SMS messaging: HTTP Basic Auth\n    Enterprise Provisioning for Marketplace HUB (CSP only): Bearer via POST /auth/login\n    Custom fields: Bearer via POST /token\n    Subscription location: Bearer via POST /token\n    Subscription signaling usages: Bearer via POST /token\n    Subscription signaling events: Bearer via POST /token\n    'Devices: eUICC inventory view': Bearer via POST /token\n    AerAdmin / AerFrame / AerTraffic (Aeris-native): apiKey query parameter\n  jwt_claims:\n\
  \  - sub\n  - iss\n  - aud\n  - azp\n  - upn\n  - email\n  - first_name\n  - last_name\n  - groups\n  - organization_ids\n  - enterprise_group_ids\n  - billing_organization_id\n  - exp\n  - iat\n  - jti\n  token_reuse_guidance: Aeris documents reading the exp claim and reusing the token rather than re-authenticating\n    per request; /iot/api/auth is rate limited to 5 req/s and 60 req/min.\n  onboarding: Credentials are issued by the Connectivity Service Provider on subscription; there is no self-serve\n    API key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aeris/refs/heads/main/authentication/aeris-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- IoT
- Cellular Connectivity
- M2M
- eSIM
- SIM Management
- Telecom
- Device Management
- IoT Security
- Connectivity Management Platform
- SMS Messaging
- eUICC
- Fleet Telematics
---
