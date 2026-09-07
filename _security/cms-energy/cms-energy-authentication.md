---
anonymous_access: true
api_key_in: []
api_specs:
- filename: cms-energy-authorizations-api-openapi.yml
  format: yaml
  label: CMS Energy Authorizations API
  slug: cms-energy-authorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-energy/refs/heads/main/openapi/cms-energy-authorizations-api-openapi.yml
- filename: cms-energy-bills-api-openapi.yml
  format: yaml
  label: CMS Energy Bills API
  slug: cms-energy-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-energy/refs/heads/main/openapi/cms-energy-bills-api-openapi.yml
- filename: cms-energy-greenbutton-api-openapi.yml
  format: yaml
  label: CMS Energy GreenButton API
  slug: cms-energy-greenbutton-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-energy/refs/heads/main/openapi/cms-energy-greenbutton-api-openapi.yml
- filename: cms-energy-intervals-api-openapi.yml
  format: yaml
  label: CMS Energy Intervals API
  slug: cms-energy-intervals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-energy/refs/heads/main/openapi/cms-energy-intervals-api-openapi.yml
- filename: cms-energy-meters-api-openapi.yml
  format: yaml
  label: CMS Energy Meters API
  slug: cms-energy-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-energy/refs/heads/main/openapi/cms-energy-meters-api-openapi.yml
- filename: cms-energy-outage-map-api-openapi.yml
  format: yaml
  label: Consumers Energy Outage Map ArcGIS REST API
  slug: cms-energy-outage-map-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-energy/refs/heads/main/openapi/cms-energy-outage-map-api-openapi.yml
auth_types:
- none
- http
- oauth2
description: 'Authentication across the two CMS Energy API surfaces. They could not be more different: the Consumers Energy ArcGIS outage services are fully anonymous, and the Consumers Energy Green Button Connect My Data program is doubly gated — a human-reviewed third-party registration with Consumers Energy, and then a per-customer OAuth authorization on top of it.'
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Cms Energy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- clientCredentials
overview: CMS Energy secures its APIs with none, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and clientCredentials flow(s).
provider_name: CMS Energy
provider_slug: cms-energy
scheme_count: 4
schemes:
- applies_to: Consumers Energy ArcGIS outage services
  name: none
  type: none
- alternative:
    in: query
    note: Documented and supported, but it puts a credential in the URL — prefer the header. Tokens are generated and expired from user settings.
    parameter: access_token
  applies_to: Consumers Energy GBCMD JSON API
  backwards_compatible_with: The same JSON API token also authenticates every Green Button API endpoint, and a logged-in dashboard session cookie works too.
  format: Bearer <api_token>
  header: Authorization
  in: header
  name: apiToken
  scheme: bearer
  source: https://utilityapi.com/docs/authentication
  type: http
- applies_to: Consumers Energy Green Button REST API
  flows:
  - access_token_lifetime_seconds: 3600
    authorizationUrl_pattern: https://utilityapi.com/DataCustodian/{utility}/oauth/authorize
    client_auth: 'HTTP Basic (client_id : client_secret)'
    flow: authorizationCode
    grant_type: authorization_code
    note: The exact CONSUMERSENERGY authorize and token URLs are per-third-party and are shown in the third party's settings only after Consumers Energy approves the registration, so they cannot be published here. The documented example uses the `demo` utility.
    refresh: grant_type=refresh_token against the same token endpoint
    scopes: see scopes/cms-energy-scopes.yml
    tokenUrl_pattern: https://utilityapi.com/DataCustodian/{utility}/oauth/token
  - flow: clientCredentials
    grant_type: client_credentials
    issues: client_access_token
  name: oauth2
  source: https://utilityapi.com/docs/greenbutton/oauth
  type: oauth2
- applies_to: Consumers Energy Green Button REST API
  classes:
  - expiry: none unless rotated
    grants: Registration endpoints
    name: registration_access_token
  - grants: Authorization and Bulk endpoints
    issued_by: client_credentials
    name: client_access_token
  - expiry_seconds: 3600
    grants: Resource and Batch endpoints for one authorization
    issued_by: authorization_code
    name: access_token
  failure_mode: Presenting a valid token of the WRONG class returns 403, not 401. 401 means missing, expired or invalid.
  name: espiTokenClasses
  scheme: bearer
  source: https://utilityapi.com/docs/greenbutton/api
  type: http
slug: cms-energy-authentication
source_filename: cms-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://utilityapi.com/docs/authentication\ndocs:\n  - https://utilityapi.com/docs/authentication\n  - https://utilityapi.com/docs/greenbutton/api\n  - https://utilityapi.com/docs/greenbutton/oauth\n  - https://utilityapi.com/docs/utilities/consumersenergy\ndescription: >-\n  Authentication across the two CMS Energy API surfaces. They could not be more different: the\n  Consumers Energy ArcGIS outage services are fully anonymous, and the Consumers Energy Green\n  Button Connect My Data program is doubly gated — a human-reviewed third-party registration\n  with Consumers Energy, and then a per-customer OAuth authorization on top of it.\nsummary:\n  types: [none, http, oauth2]\n  oauth2_flows: [authorizationCode, refreshToken, clientCredentials]\n  anonymous_surface: true\n  gated_surface: true\nsurfaces:\n  - name: Consumers Energy ArcGIS outage services\n    base: https://www.consumersenergy.com/arcgispublic/rest\n    auth:\
  \ none\n    verified: probed\n    evidence:\n      - url: https://www.consumersenergy.com/arcgispublic/rest/services/ServiceDashboard/MapServer/3/query?where=1%3D1&returnCountOnly=true&f=json\n        status: 200\n        note: Answered anonymously with real data.\n    token_service:\n      url: https://www.consumersenergy.com/arcgispublic/tokens/\n      short_lived_token_validity_minutes: 60\n      note: >-\n        ArcGIS reports isTokenBasedSecurity true at /rest/info, but every read probed answered\n        without a token. The token service is presumably for the editing capabilities the\n        FeatureServer advertises; none were exercised.\n      source: https://www.consumersenergy.com/arcgispublic/rest/info?f=json\n  - name: Consumers Energy GBCMD JSON API\n    base: https://utilityapi.com/api/v2\n    auth: bearer api token\n    operator: UtilityAPI, under licence to Consumers Energy\n  - name: Consumers Energy Green Button REST API (OpenESPI)\n    base: https://utilityapi.com/DataCustodian/espi/1_1/resource\n\
  \    auth: bearer, one of three ESPI token classes\n    operator: UtilityAPI, under licence to Consumers Energy\nschemes:\n  - name: none\n    type: none\n    applies_to: Consumers Energy ArcGIS outage services\n  - name: apiToken\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Bearer <api_token>'\n    alternative:\n      in: query\n      parameter: access_token\n      note: >-\n        Documented and supported, but it puts a credential in the URL — prefer the header. Tokens\n        are generated and expired from user settings.\n    applies_to: Consumers Energy GBCMD JSON API\n    backwards_compatible_with: >-\n      The same JSON API token also authenticates every Green Button API endpoint, and a logged-in\n      dashboard session cookie works too.\n    source: https://utilityapi.com/docs/authentication\n  - name: oauth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        grant_type: authorization_code\n        authorizationUrl_pattern:\
  \ https://utilityapi.com/DataCustodian/{utility}/oauth/authorize\n        tokenUrl_pattern: https://utilityapi.com/DataCustodian/{utility}/oauth/token\n        client_auth: \"HTTP Basic (client_id : client_secret)\"\n        access_token_lifetime_seconds: 3600\n        refresh: grant_type=refresh_token against the same token endpoint\n        scopes: see scopes/cms-energy-scopes.yml\n        note: >-\n          The exact CONSUMERSENERGY authorize and token URLs are per-third-party and are shown in\n          the third party's settings only after Consumers Energy approves the registration, so\n          they cannot be published here. The documented example uses the `demo` utility.\n      - flow: clientCredentials\n        grant_type: client_credentials\n        issues: client_access_token\n    applies_to: Consumers Energy Green Button REST API\n    source: https://utilityapi.com/docs/greenbutton/oauth\n  - name: espiTokenClasses\n    type: http\n    scheme: bearer\n    applies_to: Consumers\
  \ Energy Green Button REST API\n    classes:\n      - name: registration_access_token\n        grants: Registration endpoints\n        expiry: none unless rotated\n      - name: client_access_token\n        grants: Authorization and Bulk endpoints\n        issued_by: client_credentials\n      - name: access_token\n        grants: Resource and Batch endpoints for one authorization\n        issued_by: authorization_code\n        expiry_seconds: 3600\n    failure_mode: >-\n      Presenting a valid token of the WRONG class returns 403, not 401. 401 means missing,\n      expired or invalid.\n    source: https://utilityapi.com/docs/greenbutton/api\nend_user_authentication:\n  method: Consumers Energy single sign-on\n  described_as: OpenIDConnect\n  default: true\n  scope_value: AdditionalScope=auth-sso\n  force_login: Add prompt=on to the authorize URL to skip session reuse.\n  second_factor: >-\n    The utility may send a confirmation code by text or email as a second factor during\n    authorization.\n\
  \  test_bypass: AdditionalScope=auth-test-{test_residential|test_commercial|test_empty}\n  source: https://utilityapi.com/docs/utilities/consumersenergy\nonboarding_gate:\n  self_serve: false\n  detail: >-\n    A third party must register with Consumers Energy and is issued a client_id. Registration\n    starts in sandbox mode and only reaches live data after Consumers Energy reviews it and sends\n    an approval email. There is no self-serve path to production.\n  registration_url: https://greenbutton.consumersenergy.com/third-party/register\n  utility_id: CONSUMERSENERGY\ndiscovery_documents:\n  openid_configuration: false\n  oauth_authorization_server: false\n  oauth_protected_resource: false\n  note: >-\n    None served on any host probed — see well-known/cms-energy-well-known.yml. A client cannot\n    discover the endpoints; it must read them out of its own settings page.\ndefects:\n  - field: tokenUrl\n    value: https://utilityapi.com/api/v2/oauth/token\n    found_in: openapi/*-openapi.yml\
  \ securitySchemes.oauth2\n    probe_status: 404\n    detail: >-\n      This URL is carried in the OpenAPI securitySchemes in this repo and does not exist. It was\n      authored into the scaffolded spec rather than harvested. The real token endpoint is the\n      per-utility DataCustodian path. Recorded here rather than silently patched.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cms-energy/refs/heads/main/authentication/cms-energy-authentication.yml
summary_line: none/http/oauth2 · 4 schemes
tags:
- Electric
- Energy
- Green Button
- Michigan
- Natural Gas
- Utility
- Fortune 500
---
