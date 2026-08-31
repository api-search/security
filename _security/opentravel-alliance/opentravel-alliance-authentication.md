---
api_key_in: []
api_specs:
- filename: opentravel-alliance-facilities-api-openapi.yml
  format: yaml
  label: OpenTravel Alliance Facilities API
  slug: opentravel-alliance-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentravel-alliance/refs/heads/main/openapi/opentravel-alliance-facilities-api-openapi.yml
- filename: opentravel-alliance-hospitalityfindhospitalityavailability-api-openapi.yml
  format: yaml
  label: OpenTravel Alliance Hospitality Find Hospitality Availability API
  slug: opentravel-alliance-hospitalityfindhospitalityavailability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentravel-alliance/refs/heads/main/openapi/opentravel-alliance-hospitalityfindhospitalityavailability-api-openapi.yml
- filename: opentravel-alliance-hospitalityoffers-api-openapi.yml
  format: yaml
  label: OpenTravel Alliance Hospitality Offers API
  slug: opentravel-alliance-hospitalityoffers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentravel-alliance/refs/heads/main/openapi/opentravel-alliance-hospitalityoffers-api-openapi.yml
- filename: opentravel-alliance-hospitalitypropertyoffers-api-openapi.yml
  format: yaml
  label: OpenTravel Alliance Hospitality Property Offers API
  slug: opentravel-alliance-hospitalitypropertyoffers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentravel-alliance/refs/heads/main/openapi/opentravel-alliance-hospitalitypropertyoffers-api-openapi.yml
- filename: opentravel-alliance-hospitalityretrievefacilityavailability-api-openapi.yml
  format: yaml
  label: OpenTravel Alliance Hospitality Retrieve Facility Availability API
  slug: opentravel-alliance-hospitalityretrievefacilityavailability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentravel-alliance/refs/heads/main/openapi/opentravel-alliance-hospitalityretrievefacilityavailability-api-openapi.yml
- filename: opentravel-alliance-hoteldescriptivecontents-api-openapi.yml
  format: yaml
  label: OpenTravel Alliance Hotel Descriptive Contents API
  slug: opentravel-alliance-hoteldescriptivecontents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentravel-alliance/refs/heads/main/openapi/opentravel-alliance-hoteldescriptivecontents-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Opentravel Alliance Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: OpenTravel Alliance secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: OpenTravel Alliance
provider_slug: opentravel-alliance
scheme_count: 1
schemes:
- bearer_methods_supported:
  - header
  client_registration: No registration_endpoint is advertised; the authorization server sets client_id_metadata_document_supported=true (client ID metadata documents, the OAuth client-id-as-URL pattern) instead of RFC 7591 dynamic client registration.
  flows:
  - authorizationUrl: https://opentravel.org/oauth/authorize
    flow: authorizationCode
    revocationUrl: https://opentravel.org/oauth/revoke
    scopes:
      mcp: Access the OpenTravel Model Context Protocol server
    tokenUrl: https://opentravel.org/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  name: opentravel-mcp-oauth
  pkce:
    required_methods:
    - S256
  protects:
  - https://opentravel.org/wp-json/mcp/mcp-oauth-server
  - https://opentravel.org/wp-json/mcp/mcp-adapter-default-server
  sources:
  - well-known/opentravel-alliance-oauth-authorization-server.json
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: opentravel-alliance-authentication
source_filename: opentravel-alliance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource: https://opentravel.org/.well-known/oauth-authorization-server\ndocs: https://opentravel.org/.well-known/oauth-protected-resource\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  note: >-\n    Two distinct authentication stories sit under one organization. (1) The published\n    OpenTravel 2.0 Swagger contracts declare NO securityDefinitions at all — authentication is\n    left entirely to the implementer that hosts the resource. (2) opentravel.org itself runs a\n    real OAuth 2.1 authorization server in front of its Model Context Protocol endpoints.\nschemes:\n- name: opentravel-mcp-oauth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://opentravel.org/oauth/authorize\n    tokenUrl: https://opentravel.org/oauth/token\n    revocationUrl: https://opentravel.org/oauth/revoke\n    scopes:\n      mcp: Access the OpenTravel Model Context Protocol server\n\
  \  pkce:\n    required_methods: [S256]\n  grant_types_supported: [authorization_code, refresh_token]\n  token_endpoint_auth_methods_supported: [none]\n  client_registration: >-\n    No registration_endpoint is advertised; the authorization server sets\n    client_id_metadata_document_supported=true (client ID metadata documents, the OAuth\n    client-id-as-URL pattern) instead of RFC 7591 dynamic client registration.\n  bearer_methods_supported: [header]\n  protects:\n  - https://opentravel.org/wp-json/mcp/mcp-oauth-server\n  - https://opentravel.org/wp-json/mcp/mcp-adapter-default-server\n  sources: [well-known/opentravel-alliance-oauth-authorization-server.json]\nspec_declared_security:\n  schemes: []\n  evidence: >-\n    All eight harvested Swagger 2.0 documents were parsed on 2026-07-28: securityDefinitions is\n    absent and no operation carries a security requirement. The OTM compiler that generated\n    them emits the message contract only; 401 and 403 responses are declared on\
  \ every\n    operation but no scheme is named to satisfy them.\n  files:\n  - openapi/opentravel-2020a-hotel-descriptive-content-resource-openapi.json\n  - openapi/opentravel-2020a-hotel-descriptive-content-resource-defs-openapi.json\n  - openapi/opentravel-2020a-facility-resource-openapi.json\n  - openapi/opentravel-2020a-facility-resource-defs-openapi.json\n  - openapi/opentravel-2018a-hospitality-offers-resource-openapi.json\n  - openapi/opentravel-2018a-hospitality-offers-resource-defs-openapi.json\n  - openapi/opentravel-2018a-facility-resource-openapi.json\n  - openapi/opentravel-2018a-facility-resource-defs-openapi.json\nother_account_surfaces:\n- surface: OTM Library Repository console\n  url: https://opentravelmodel.net/\n  mechanism: User ID / password form login\n  api: none documented\n- surface: OpenTravel Developers Network (ODN)\n  url: https://www.opentraveldevelopersnetwork.com/user\n  mechanism: free site account (register at /user/register); member-only sections\n  api:\
  \ none documented\n- surface: WordPress REST API on opentravel.org\n  url: https://opentravel.org/wp-json/\n  mechanism: application passwords (authorization at /wp-admin/authorize-application.php)\n  api: CMS plumbing, not an OpenTravel product API\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opentravel-alliance/refs/heads/main/authentication/opentravel-alliance-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Travel
- United States
- Standards
- Aviation
- Hospitality
- Hotels
- Car Rental
- Rail
- Cruise
- Distribution
- GDS
- Booking
- Channel
- XML
- JSON-Schema
---
