---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nasdaq-asyncapi.yml
  format: yaml
  label: Nasdaq Cloud Data Service (NCDS) — Kafka Streams
  slug: nasdaq-cloud-data-service-ncds-kafka-streams
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasdaq/refs/heads/main/asyncapi/nasdaq-asyncapi.yml
- filename: nasdaq-ncds-rest-postman-collection.json
  format: json
  label: Nasdaq Cloud Data Service (NCDS) REST API
  slug: nasdaq-cloud-data-service-ncds-rest-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nasdaq/refs/heads/main/postman/nasdaq-ncds-rest-postman-collection.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Nasdaq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nasdaq declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Nasdaq
provider_slug: nasdaq
scheme_count: 4
schemes:
- applies_to: Nasdaq Data Link Tables API
  in: query
  name: api_key
  parameter: api_key
  type: apiKey
- applies_to: Nasdaq Data Link Bulk Download API
  in: header
  name: X-Api-Token
  parameter: X-Api-Token
  type: apiKey
- applies_to: NCDS REST API
  description: POST client_id and client_secret as JSON; response carries access_token and expires_in (seconds).
  name: ncds-client-credentials
  scheme: bearer
  token_url: https://<base_url>/v1/auth/token
  type: http
- applies_to: NCDS Streaming (Kafka)
  description: SASL/OAUTHBEARER against an onboarding-issued token endpoint; client ID, client secret, token endpoint and bootstrap servers are issued at onboarding.
  flow: clientCredentials
  name: ncds-kafka-oauthbearer
  type: oauth2
slug: nasdaq-authentication
source_filename: nasdaq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Nasdaq authentication\ngenerated: '2026-10-19'\nmethod: searched\nsource: https://data.nasdaq.com/tablesapi\ndocs: https://data.nasdaq.com/tablesapi\nschemes:\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  applies_to: Nasdaq Data Link Tables API\n- name: X-Api-Token\n  type: apiKey\n  in: header\n  parameter: X-Api-Token\n  applies_to: Nasdaq Data Link Bulk Download API\n- name: ncds-client-credentials\n  type: http\n  scheme: bearer\n  token_url: https://<base_url>/v1/auth/token\n  description: POST client_id and client_secret as JSON; response carries access_token\n    and expires_in (seconds).\n  applies_to: NCDS REST API\n- name: ncds-kafka-oauthbearer\n  type: oauth2\n  flow: clientCredentials\n  description: SASL/OAUTHBEARER against an onboarding-issued token endpoint; client\n    ID, client secret, token endpoint and bootstrap servers are issued at onboarding.\n  applies_to: NCDS Streaming (Kafka)\ndocs_ncds: https://github.com/Nasdaq/NasdaqCloudDataService-REST-API/blob/main/restapi/authenticate.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasdaq/refs/heads/main/authentication/nasdaq-authentication.yml
summary_line: 4 schemes
tags:
- Data Marketplace
- Financial Data
- Fortune 1000
- Kafka
- Market Data
- Stock Exchange
- Streaming
---
