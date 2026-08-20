---
api_key_in:
- header
api_specs:
- filename: traveloka-1-1-content-hotel-room-api-openapi.yml
  format: yaml
  label: Traveloka 1.1 Content - Hotel & Room API
  slug: traveloka-1-1-content-hotel-room-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-1-1-content-hotel-room-api-openapi.yml
- filename: traveloka-2-1-search-hotellist-api-openapi.yml
  format: yaml
  label: Traveloka 2.1 Search - HotelList API
  slug: traveloka-2-1-search-hotellist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-2-1-search-hotellist-api-openapi.yml
- filename: traveloka-2-2-search-roomlist-api-openapi.yml
  format: yaml
  label: Traveloka 2.2 Search - RoomList API
  slug: traveloka-2-2-search-roomlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-2-2-search-roomlist-api-openapi.yml
- filename: traveloka-2-3-search-bulkroomlist-api-openapi.yml
  format: yaml
  label: Traveloka 2.3 Search - BulkRoomList API
  slug: traveloka-2-3-search-bulkroomlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-2-3-search-bulkroomlist-api-openapi.yml
- filename: traveloka-3-1-booking-book-api-openapi.yml
  format: yaml
  label: Traveloka 3.1 Booking - Book API
  slug: traveloka-3-1-booking-book-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-3-1-booking-book-api-openapi.yml
- filename: traveloka-3-2-booking-issuecheck-api-openapi.yml
  format: yaml
  label: Traveloka 3.2 Booking - IssueCheck API
  slug: traveloka-3-2-booking-issuecheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-3-2-booking-issuecheck-api-openapi.yml
- filename: traveloka-3-3-booking-issue-api-openapi.yml
  format: yaml
  label: Traveloka 3.3 Booking - Issue API
  slug: traveloka-3-3-booking-issue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-3-3-booking-issue-api-openapi.yml
- filename: traveloka-3-4-booking-bookingsummary-api-openapi.yml
  format: yaml
  label: Traveloka 3.4 Booking - BookingSummary API
  slug: traveloka-3-4-booking-bookingsummary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-3-4-booking-bookingsummary-api-openapi.yml
- filename: traveloka-3-5-booking-cancel-api-openapi.yml
  format: yaml
  label: Traveloka 3.5 Booking - Cancel API
  slug: traveloka-3-5-booking-cancel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-3-5-booking-cancel-api-openapi.yml
- filename: traveloka-authorization-api-openapi.yml
  format: yaml
  label: Traveloka Authorization API
  slug: traveloka-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-authorization-api-openapi.yml
- filename: traveloka-booking-api-openapi.yml
  format: yaml
  label: Traveloka Booking API
  slug: traveloka-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-booking-api-openapi.yml
- filename: traveloka-content-api-openapi.yml
  format: yaml
  label: Traveloka Content API
  slug: traveloka-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-content-api-openapi.yml
- filename: traveloka-discovery-optional-api-openapi.yml
  format: yaml
  label: Traveloka Discovery (Optional) API
  slug: traveloka-discovery-optional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-discovery-optional-api-openapi.yml
- filename: traveloka-rate-api-openapi.yml
  format: yaml
  label: Traveloka Rate API
  slug: traveloka-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/openapi/traveloka-rate-api-openapi.yml
auth_types:
- oauth2
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Traveloka Authentication
name_suffix: Authentication
oauth_flows: []
overview: Traveloka secures its APIs with oauth2, apiKey, and http across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Traveloka
provider_slug: traveloka
scheme_count: 0
schemes: []
slug: traveloka-authentication
source_filename: traveloka-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: >-\n  https://developer.travelokapartnersnetwork.com/faq +\n  https://developer.travelokapartnersnetwork.com/api-docs (LOKA API v2.4.8 OpenAPI) +\n  https://atlas.traveloka.com/developers/docs/ (Traveloka Specification API) +\n  https://developer.connect.traveloka.com/api-doc/credentials/url/\ndocs: https://developer.travelokapartnersnetwork.com/api-docs\nsummary:\n  types: [oauth2, apiKey, http]\n  api_key_in: [header]\n  note: >-\n    Three distinct Traveloka API surfaces use three distinct auth models. The published LOKA v2 OpenAPI\n    declares its bearer credential as an apiKey-in-header scheme (an AWS API Gateway Lambda authorizer),\n    but the documented way to MINT that credential is an OAuth 2.0 client-credentials exchange. Both\n    facts are recorded below; neither is inferred.\n\napis:\n  - api: Traveloka Partners Network (LOKA) v2 Accommodation API\n    primary: oauth2_client_credentials\n    token_endpoint: https://auth-api.afc.traveloka.com/oauth/accesstoken\n\
  \    staging_token_endpoint: https://auth-api.afc.staging-traveloka.com/oauth/accesstoken\n    method: POST\n    request_media_type: application/x-www-form-urlencoded\n    credential_fields: [client_id, client_secret]\n    response_fields: [token_type, access_token, expires_in]\n    response_schema: AccessToken\n    token_lifetime_minutes: 60\n    token_reuse: >-\n      Reuse until expiry. The provider FAQ explicitly discourages minting a token per call.\n    transport:\n      header: Authorization\n      location: header\n      note: >-\n        The spec models this as securityScheme api_gateway_lambda_authorizer (type apiKey, in header,\n        name Authorization) fronted by an AWS API Gateway custom Lambda authorizer with a 1800-second\n        authorizer result TTL.\n    expiry_signal:\n      status: 401\n      code: '401'\n      message: Unauthorized, the token might be expired.\n      remediation: Re-issue via POST /oauth/accesstoken with the original client_id and client_secret.\n\
  \    additional_scheme:\n      name: sigv4\n      type: apiKey\n      in: header\n      parameter: Authorization\n      x-amazon-apigateway-authtype: awsSigv4\n      note: >-\n        Declared in components.securitySchemes but not applied to any operation in the published spec.\n    scopes:\n      declared: ['auth']\n      note: >-\n        The spec's root security requirement is [{\"OAuthStaging\": [\"auth\"]}] but \"OAuthStaging\" is not\n        defined in components.securitySchemes - a dangling reference in the published document. No scope\n        reference page is published, so no scopes/ artifact is emitted.\n    credential_issuance:\n      model: approval\n      steps:\n        - Choose a partnership model.\n        - Register via the Become Partner form.\n        - Formalize the partnership to receive unique site credentials.\n        - Request certification from the Traveloka connectivity team.\n        - Promote to the live environment.\n      form: https://traveloka.sg.larksuite.com/share/base/form/shrlg7CyVohw5GHPRXwt8LdPCCW\n\
  \      contact: partnersnetwork@traveloka.com\n      self_serve: false\n\n  - api: Traveloka Atlas - Traveloka Specification API (supplier-implemented)\n    primary: http_basic\n    scheme: basic\n    format: base64(username:password)\n    header: 'Authorization: Basic <base64>'\n    transport_requirement: HTTPS on port 443\n    direction: >-\n      Inverted. Traveloka is the CLIENT; the accommodation supplier hosts these endpoints and validates\n      the Basic credential Traveloka presents.\n    source_scheme: basicAuth\n    sources: [openapi/traveloka-atlas-supplier-api-openapi.yml]\n\n  - api: Traveloka Connect - Connectivity API (OTA 2017B XML)\n    primary: partner_credentials\n    base_url: https://api.connect.traveloka.com/\n    staging_base_url: https://api.connect.staging-traveloka.com/\n    issuance:\n      staging: Credentials issued after NDA signing.\n      production: Credentials issued after certification.\n      contact: tera-cm@traveloka.com\n      channels: [Lark, Email,\
  \ Teams]\n    note: >-\n      The credential mechanism itself is documented behind the developer.connect.traveloka.com login; the\n      public surface documents only the issuance process, base URLs, and OTA message set.\n    self_serve: false\n\naccess_model:\n  onboarding: approval\n  pricing: enterprise\n  public: false\n  try_now: false\n  confidence: high\n  evidence: >-\n    No self-serve signup exists for any of the three surfaces. Every path requires a partnership form,\n    contract and certification before credentials are issued.\n\ncross_links:\n  conventions: conventions/traveloka-conventions.yml\n  sandbox: sandbox/traveloka-sandbox.yml\n  errors: errors/traveloka-problem-types.yml\n  conformance: conformance/traveloka-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/traveloka/refs/heads/main/authentication/traveloka-authentication.yml
summary_line: oauth2/apiKey/http · 0 schemes
tags:
- Travel
- Online Travel Agency
- Accommodation
- Hotel Booking
- Flights
- Activities
- Hospitality
- Distribution
- Channel Manager
- OpenTravel
- Southeast Asia
- Indonesia
---
