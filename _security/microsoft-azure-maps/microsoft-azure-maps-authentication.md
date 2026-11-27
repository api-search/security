---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: microsoft-azure-maps-search-api-openapi.yml
  format: yaml
  label: Azure Maps Search API
  slug: microsoft-azure-maps-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-search-api-openapi.yml
- filename: microsoft-azure-maps-geocode-api-openapi.yml
  format: yaml
  label: Azure Maps Geocode API
  slug: microsoft-azure-maps-geocode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-geocode-api-openapi.yml
- filename: microsoft-azure-maps-geocode-autocomplete-api-openapi.yml
  format: yaml
  label: Azure Maps Geocode:autocomplete API
  slug: microsoft-azure-maps-geocode-autocomplete-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-geocode-autocomplete-api-openapi.yml
- filename: microsoft-azure-maps-geocode-batch-api-openapi.yml
  format: yaml
  label: Azure Maps Geocode:batch API
  slug: microsoft-azure-maps-geocode-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-geocode-batch-api-openapi.yml
- filename: microsoft-azure-maps-geolocation-api-openapi.yml
  format: yaml
  label: Azure Maps Geolocation API
  slug: microsoft-azure-maps-geolocation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-geolocation-api-openapi.yml
- filename: microsoft-azure-maps-map-api-openapi.yml
  format: yaml
  label: Azure Maps Map API
  slug: microsoft-azure-maps-map-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-map-api-openapi.yml
- filename: microsoft-azure-maps-reversegeocode-api-openapi.yml
  format: yaml
  label: Azure Maps Reverse Geocode API
  slug: microsoft-azure-maps-reversegeocode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-reversegeocode-api-openapi.yml
- filename: microsoft-azure-maps-reversegeocode-batch-api-openapi.yml
  format: yaml
  label: Azure Maps Reverse Geocode:batch API
  slug: microsoft-azure-maps-reversegeocode-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-reversegeocode-batch-api-openapi.yml
- filename: microsoft-azure-maps-route-api-openapi.yml
  format: yaml
  label: Azure Maps Route API
  slug: microsoft-azure-maps-route-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-route-api-openapi.yml
- filename: microsoft-azure-maps-timezone-api-openapi.yml
  format: yaml
  label: Azure Maps Timezone API
  slug: microsoft-azure-maps-timezone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-timezone-api-openapi.yml
- filename: microsoft-azure-maps-traffic-api-openapi.yml
  format: yaml
  label: Azure Maps Traffic API
  slug: microsoft-azure-maps-traffic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-traffic-api-openapi.yml
- filename: microsoft-azure-maps-weather-api-openapi.yml
  format: yaml
  label: Azure Maps Weather API
  slug: microsoft-azure-maps-weather-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-weather-api-openapi.yml
- filename: microsoft-azure-maps-accounts-api-openapi.yml
  format: yaml
  label: Azure Maps Accounts API
  slug: microsoft-azure-maps-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-accounts-api-openapi.yml
- filename: microsoft-azure-maps-creators-api-openapi.yml
  format: yaml
  label: Azure Maps Creators API
  slug: microsoft-azure-maps-creators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-creators-api-openapi.yml
- filename: microsoft-azure-maps-operations-api-openapi.yml
  format: yaml
  label: Azure Maps Operations API
  slug: microsoft-azure-maps-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-operations-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: derived
name: Azure Maps Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Maps secures its APIs with apiKey and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Maps
provider_slug: microsoft-azure-maps
scheme_count: 4
schemes:
- in: query
  name: subscriptionKey
  parameter: subscription-key
  sources:
  - openapi/_superseded/microsoft-azure-maps-geocoding-api-openapi.yml
  - openapi/_superseded/microsoft-azure-maps-search-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/_superseded/microsoft-azure-maps-geocoding-api-openapi.yml
  - openapi/microsoft-azure-maps-geolocation-openapi.yml
  - openapi/microsoft-azure-maps-render-openapi.yml
  - openapi/microsoft-azure-maps-route-openapi.yml
  - openapi/_superseded/microsoft-azure-maps-search-api-openapi.yml
  - openapi/microsoft-azure-maps-search-openapi.yml
  - openapi/microsoft-azure-maps-timezone-openapi.yml
  - openapi/microsoft-azure-maps-traffic-openapi.yml
  - openapi/microsoft-azure-maps-weather-openapi.yml
  type: oauth2
- description: 'This is a shared access signature token created from the List SAS operation on the [Azure Maps resource](https://aka.ms/amauth) through the Azure management plane via Azure portal, PowerShell, CLI, Azure SDKs, or REST APIs.


    With this token, any application is authorized to access with Azure role-based access controls and fine-grain control to the expiration, rate, and region(s) of use for the par'
  in: header
  name: SasToken
  parameter: SAS Token
  sources:
  - openapi/microsoft-azure-maps-geolocation-openapi.yml
  - openapi/microsoft-azure-maps-render-openapi.yml
  - openapi/microsoft-azure-maps-route-openapi.yml
  - openapi/microsoft-azure-maps-search-openapi.yml
  - openapi/microsoft-azure-maps-timezone-openapi.yml
  - openapi/microsoft-azure-maps-traffic-openapi.yml
  - openapi/microsoft-azure-maps-weather-openapi.yml
  type: apiKey
- description: 'This is a shared key that is provisioned when you [Create an Azure Maps account](https://docs.microsoft.com/azure/azure-maps/quick-demo-map-app#create-an-azure-maps-account) in the Azure portal or using PowerShell, CLI, Azure SDKs, or REST API.


    With this key, any application can access all REST API. In other words, this key can be used as a master key in the account that they are issued in.


    For '
  in: header
  name: SharedKey
  parameter: subscription-key
  sources:
  - openapi/microsoft-azure-maps-geolocation-openapi.yml
  - openapi/microsoft-azure-maps-render-openapi.yml
  - openapi/microsoft-azure-maps-route-openapi.yml
  - openapi/microsoft-azure-maps-search-openapi.yml
  - openapi/microsoft-azure-maps-timezone-openapi.yml
  - openapi/microsoft-azure-maps-traffic-openapi.yml
  - openapi/microsoft-azure-maps-weather-openapi.yml
  type: apiKey
slug: microsoft-azure-maps-authentication
source_filename: microsoft-azure-maps-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/_superseded/microsoft-azure-maps-geocoding-api-openapi.yml, openapi/microsoft-azure-maps-geolocation-openapi.yml,\n  openapi/microsoft-azure-maps-render-openapi.yml, openapi/microsoft-azure-maps-route-openapi.yml,\n  openapi/_superseded/microsoft-azure-maps-search-api-openapi.yml, openapi/microsoft-azure-maps-search-openapi.yml,\n  openapi/microsoft-azure-maps-timezone-openapi.yml, openapi/microsoft-azure-maps-traffic-openapi.yml,\n  openapi/microsoft-azure-maps-weather-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - implicit\nschemes:\n- name: subscriptionKey\n  type: apiKey\n  in: query\n  parameter: subscription-key\n  sources:\n  - openapi/_superseded/microsoft-azure-maps-geocoding-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-maps-search-api-openapi.yml\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl:\
  \ https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  sources:\n  - openapi/_superseded/microsoft-azure-maps-geocoding-api-openapi.yml\n  - openapi/microsoft-azure-maps-geolocation-openapi.yml\n  - openapi/microsoft-azure-maps-render-openapi.yml\n  - openapi/microsoft-azure-maps-route-openapi.yml\n  - openapi/_superseded/microsoft-azure-maps-search-api-openapi.yml\n  - openapi/microsoft-azure-maps-search-openapi.yml\n  - openapi/microsoft-azure-maps-timezone-openapi.yml\n  - openapi/microsoft-azure-maps-traffic-openapi.yml\n  - openapi/microsoft-azure-maps-weather-openapi.yml\n- name: SasToken\n  type: apiKey\n  in: header\n  parameter: SAS Token\n  description: |-\n    This is a shared access signature token created from the List SAS operation on the [Azure Maps resource](https://aka.ms/amauth) through the Azure management plane via Azure portal, PowerShell, CLI, Azure SDKs, or REST APIs.\n\n    With this token, any application is authorized to access with Azure\
  \ role-based access controls and fine-grain control to the expiration, rate, and region(s) of use for the par\n  sources:\n  - openapi/microsoft-azure-maps-geolocation-openapi.yml\n  - openapi/microsoft-azure-maps-render-openapi.yml\n  - openapi/microsoft-azure-maps-route-openapi.yml\n  - openapi/microsoft-azure-maps-search-openapi.yml\n  - openapi/microsoft-azure-maps-timezone-openapi.yml\n  - openapi/microsoft-azure-maps-traffic-openapi.yml\n  - openapi/microsoft-azure-maps-weather-openapi.yml\n- name: SharedKey\n  type: apiKey\n  in: header\n  parameter: subscription-key\n  description: \"This is a shared key that is provisioned when you [Create an Azure Maps account](https://docs.microsoft.com/azure/azure-maps/quick-demo-map-app#create-an-azure-maps-account)\\\n    \\ in the Azure portal or using PowerShell, CLI, Azure SDKs, or REST API.\\n\\nWith this key,\\\n    \\ any application can access all REST API. In other words, this key can be used as a master\\\n    \\ key in the account\
  \ that they are issued in.\\n\\nFor \"\n  sources:\n  - openapi/microsoft-azure-maps-geolocation-openapi.yml\n  - openapi/microsoft-azure-maps-render-openapi.yml\n  - openapi/microsoft-azure-maps-route-openapi.yml\n  - openapi/microsoft-azure-maps-search-openapi.yml\n  - openapi/microsoft-azure-maps-timezone-openapi.yml\n  - openapi/microsoft-azure-maps-traffic-openapi.yml\n  - openapi/microsoft-azure-maps-weather-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-maps/authentication/microsoft-azure-maps-authentication.yml
summary_line: apiKey/oauth2 · 4 schemes
tags:
- Geocoding
- Geospatial
- Location
- Maps
- Mobility
- Routing
- Traffic
- Weather
---
