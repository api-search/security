---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: companies-house-charges-api-openapi.yml
  format: yaml
  label: Companies House Charges API
  slug: companies-house-charges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-charges-api-openapi.yml
- filename: companies-house-companyprofile-api-openapi.yml
  format: yaml
  label: Companies House Company Profile API
  slug: companies-house-companyprofile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-companyprofile-api-openapi.yml
- filename: companies-house-documentlocation-api-openapi.yml
  format: yaml
  label: Companies House Document Location API
  slug: companies-house-documentlocation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-documentlocation-api-openapi.yml
- filename: companies-house-documentmetadata-api-openapi.yml
  format: yaml
  label: Companies House Document Metadata API
  slug: companies-house-documentmetadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-documentmetadata-api-openapi.yml
- filename: companies-house-exemptions-api-openapi.yml
  format: yaml
  label: Companies House Exemptions API
  slug: companies-house-exemptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-exemptions-api-openapi.yml
- filename: companies-house-filinghistory-api-openapi.yml
  format: yaml
  label: Companies House Filing History API
  slug: companies-house-filinghistory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-filinghistory-api-openapi.yml
- filename: companies-house-insolvency-api-openapi.yml
  format: yaml
  label: Companies House Insolvency API
  slug: companies-house-insolvency-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-insolvency-api-openapi.yml
- filename: companies-house-officerappointments-api-openapi.yml
  format: yaml
  label: Companies House Officer Appointments API
  slug: companies-house-officerappointments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-officerappointments-api-openapi.yml
- filename: companies-house-officerdisqualifications-api-openapi.yml
  format: yaml
  label: Companies House Officer Disqualifications API
  slug: companies-house-officerdisqualifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-officerdisqualifications-api-openapi.yml
- filename: companies-house-officers-api-openapi.yml
  format: yaml
  label: Companies House Officers API
  slug: companies-house-officers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-officers-api-openapi.yml
- filename: companies-house-personswithsignificantcontrol-api-openapi.yml
  format: yaml
  label: Companies House Persons With Significant Control API
  slug: companies-house-personswithsignificantcontrol-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-personswithsignificantcontrol-api-openapi.yml
- filename: companies-house-personswithsignificantcontrolnotifications-api-openapi.yml
  format: yaml
  label: Companies House Persons With Significant Control Notifications API
  slug: companies-house-personswithsignificantcontrolnotifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-personswithsignificantcontrolnotifications-api-openapi.yml
- filename: companies-house-registeredofficeaddress-api-openapi.yml
  format: yaml
  label: Companies House Registered Office Address API
  slug: companies-house-registeredofficeaddress-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-registeredofficeaddress-api-openapi.yml
- filename: companies-house-registers-api-openapi.yml
  format: yaml
  label: Companies House Registers API
  slug: companies-house-registers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-registers-api-openapi.yml
- filename: companies-house-search-api-openapi.yml
  format: yaml
  label: Companies House Search API
  slug: companies-house-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-search-api-openapi.yml
- filename: companies-house-ukestablishments-api-openapi.yml
  format: yaml
  label: Companies House UK Establishments API
  slug: companies-house-ukestablishments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-ukestablishments-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Companies House Authentication
name_suffix: Authentication
oauth_flows: []
overview: Companies House secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Companies House
provider_slug: companies-house
scheme_count: 3
schemes:
- description: 'API key sent in the HTTP Authorization header using Basic authentication. The API key is the username; the password is left blank. Used for GET requests to the Public Data API and Document API.

    '
  example: 'Authorization: Basic bXlfYXBpX2tleTo='
  in: header
  name: api_key
  parameter: Authorization
  scheme: Basic
  sources:
  - https://developer.company-information.service.gov.uk/authentication
  - https://developer-specs.company-information.service.gov.uk/guides/authorisation
  - openapi/companies-house-public-data-api-openapi.yml
  - openapi/companies-house-document-api-openapi.yml
  type: apiKey
- description: 'Stream key sent in the HTTP Authorization header using Basic authentication (same mechanism as api_key). Issued as a separate credential type for Streaming API connections. Each account is limited to two concurrent streaming connections.

    '
  in: header
  name: stream_key
  parameter: Authorization
  scheme: Basic
  sources:
  - https://developer.company-information.service.gov.uk/authentication
  - openapi/companies-house-streaming-api-openapi.yml
  type: apiKey
- authorization_url: https://identity.company-information.service.gov.uk/oauth2/authorise
  description: 'OAuth 2.0 authorization_code flow for end-user interaction with filing and account-scoped functionality. Developers register an OAuth web client in the Developer Hub to obtain a client_id and client_secret. The end user signs in to Companies House and may be required to provide a Company authentication code when the requested scopes contain a specific company number. Access tokens can be refreshed using the refresh_token grant. The Authorization header carries a Bearer token.

    '
  example: 'Authorization: Bearer my_access_token'
  flow: authorizationCode
  grants:
  - authorization_code
  - refresh_token
  name: oauth2
  sources:
  - https://developer.company-information.service.gov.uk/authentication
  - https://developer-specs.company-information.service.gov.uk/guides/authorisation
  token_type: Bearer
  token_url: https://identity.company-information.service.gov.uk/oauth2/token
  type: oauth2
  verify_url: https://identity.company-information.service.gov.uk/oauth2/verify
slug: companies-house-authentication
source_filename: companies-house-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: searched\nsource: https://developer.company-information.service.gov.uk/authentication\ndocs: https://developer.company-information.service.gov.uk/authentication\nrelated_docs:\n- https://developer-specs.company-information.service.gov.uk/guides/authorisation\n- https://developer.company-information.service.gov.uk/how-to-create-an-application\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  note: >\n    Three client credential types are issued by the Companies House Developer Hub:\n    API key, stream key, and OAuth web client. API key and stream key are transmitted\n    using HTTP Basic access authentication (RFC 2617) — the key is placed in the\n    username position of the Basic credential and the password is left blank. OAuth\n    web clients use HTTP Bearer authentication with an access token obtained through\n    the OAuth 2.0 authorization_code grant.\nschemes:\n- name: api_key\n  type: apiKey\n  in:\
  \ header\n  parameter: Authorization\n  scheme: Basic\n  description: >\n    API key sent in the HTTP Authorization header using Basic authentication. The\n    API key is the username; the password is left blank. Used for GET requests to\n    the Public Data API and Document API.\n  example: 'Authorization: Basic bXlfYXBpX2tleTo='\n  sources:\n  - https://developer.company-information.service.gov.uk/authentication\n  - https://developer-specs.company-information.service.gov.uk/guides/authorisation\n  - openapi/companies-house-public-data-api-openapi.yml\n  - openapi/companies-house-document-api-openapi.yml\n- name: stream_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  scheme: Basic\n  description: >\n    Stream key sent in the HTTP Authorization header using Basic authentication\n    (same mechanism as api_key). Issued as a separate credential type for Streaming\n    API connections. Each account is limited to two concurrent streaming connections.\n  sources:\n  - https://developer.company-information.service.gov.uk/authentication\n\
  \  - openapi/companies-house-streaming-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  authorization_url: https://identity.company-information.service.gov.uk/oauth2/authorise\n  token_url: https://identity.company-information.service.gov.uk/oauth2/token\n  verify_url: https://identity.company-information.service.gov.uk/oauth2/verify\n  description: >\n    OAuth 2.0 authorization_code flow for end-user interaction with filing and\n    account-scoped functionality. Developers register an OAuth web client in the\n    Developer Hub to obtain a client_id and client_secret. The end user signs in\n    to Companies House and may be required to provide a Company authentication\n    code when the requested scopes contain a specific company number. Access tokens\n    can be refreshed using the refresh_token grant. The Authorization header carries\n    a Bearer token.\n  grants:\n  - authorization_code\n  - refresh_token\n  token_type: Bearer\n  example: 'Authorization:\
  \ Bearer my_access_token'\n  sources:\n  - https://developer.company-information.service.gov.uk/authentication\n  - https://developer-specs.company-information.service.gov.uk/guides/authorisation\nnotes:\n- The OAuth 2.0 service URLs above are the identity-service hosts referenced in\n  the sandbox docs; the live identity host is identity.company-information.service.gov.uk\n  and the sandbox host is identity-sandbox.company-information.service.gov.uk.\n"
source_yaml_url: https://artifacts.apis.io/companies-house/authentication/companies-house-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Companies
- UK Government
- Business Registration
- Company Search
- Officers
- Filing History
- Insolvency
- Charges
- Persons of Significant Control
- Open Data
---
