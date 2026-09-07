---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: accruent-maintenance-connection-openapi.yml
  format: yaml
  label: Maintenance Connection Web API
  slug: maintenance-connection-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accruent/refs/heads/main/openapi/accruent-maintenance-connection-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Accruent Authentication
name_suffix: Authentication
oauth_flows: []
overview: Accruent secures its APIs with http and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Accruent
provider_slug: accruent
scheme_count: 4
schemes:
- applies_to: Maintenance Connection Web API
  description: HTTP Basic. The Authorization header carries base64("ConnectionKey:APIKey") after the "Basic " prefix, where the Connection Key identifies the Maintenance Connection database and the API key is issued by Accruent for that database. A missing or malformed header returns 401 Unauthorized; a non-SSL request also returns 401.
  docs: https://api.maintenanceconnection.com/v8/help/docs/AuthenticationDocs
  name: basic
  scheme: basic
  sources:
  - openapi/accruent-maintenance-connection-openapi.yml
  spec_applied: false
  type: http
- alternate:
    in: query
    parameter_name: subscription-key
  applies_to: Siterra API
  description: Azure API Management subscription key for the Siterra API on the Accruent Developer Network. Keys are issued only after an invitation into the Accruent Developer Program is approved.
  docs: https://developer.accruent.com/wiki/siterra/gettingstarted
  in: header
  method: searched
  name: accruent-subscription-key
  parameter_name: accruent-subscription-key
  type: apiKey
- alternate:
    in: query
    parameter_name: subscription-key
  applies_to: Meridian Cloud API
  description: Azure API Management subscription key for the Meridian Cloud API. Subscriptions are requested from the Products page of the regional Meridian developer portal and activated on approval.
  docs: https://api-developer.meridiancloud.net/wiki/meridian/gettingstarted
  in: header
  method: searched
  name: Ocp-Apim-Subscription-Key
  parameter_name: Ocp-Apim-Subscription-Key
  type: apiKey
- applies_to: EMS Platform Services
  bearerFormat: JWT
  description: EMS Platform Services requires a valid JWT authentication token on every API resource call. Tokens are issued inside the customer tenancy; the legacy EMS SOAP API Web Service it replaces authenticates with a predefined EMS user account instead.
  docs: https://help.accruent.com/ems/Content/EMSPlatformServices/InstallationGuide/Introduction.html
  method: searched
  name: ems-platform-jwt
  scheme: bearer
  type: http
slug: accruent-authentication
source_filename: accruent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: openapi/accruent-maintenance-connection-openapi.yml\ndocs: https://api.maintenanceconnection.com/v8/help/docs/AuthenticationDocs\nnote: >-\n  Derived from the Maintenance Connection Swagger 2.0 securityDefinitions, then upgraded from the\n  published auth pages for each Accruent product surface. Accruent runs four different auth models\n  across its portfolio; only Maintenance Connection publishes its scheme in a machine-readable\n  contract, and even there the basic scheme is DEFINED but never APPLIED to any of the 255\n  operations (no top-level or per-operation security[] block), so a generator reading the spec\n  alone would emit an unauthenticated client.\nsummary:\n  types:\n  - http\n  - apiKey\n  http_schemes:\n  - basic\n  api_key_in:\n  - header\n  - query\n  oauth2_flows: []\nschemes:\n- name: basic\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic. The Authorization header carries base64(\"ConnectionKey:APIKey\"\
  ) after the \"Basic \"\n    prefix, where the Connection Key identifies the Maintenance Connection database and the API key\n    is issued by Accruent for that database. A missing or malformed header returns 401 Unauthorized;\n    a non-SSL request also returns 401.\n  applies_to: Maintenance Connection Web API\n  docs: https://api.maintenanceconnection.com/v8/help/docs/AuthenticationDocs\n  sources:\n  - openapi/accruent-maintenance-connection-openapi.yml\n  spec_applied: false\n- name: accruent-subscription-key\n  type: apiKey\n  in: header\n  parameter_name: accruent-subscription-key\n  alternate:\n    in: query\n    parameter_name: subscription-key\n  description: >-\n    Azure API Management subscription key for the Siterra API on the Accruent Developer Network.\n    Keys are issued only after an invitation into the Accruent Developer Program is approved.\n  applies_to: Siterra API\n  docs: https://developer.accruent.com/wiki/siterra/gettingstarted\n  method: searched\n- name: Ocp-Apim-Subscription-Key\n\
  \  type: apiKey\n  in: header\n  parameter_name: Ocp-Apim-Subscription-Key\n  alternate:\n    in: query\n    parameter_name: subscription-key\n  description: >-\n    Azure API Management subscription key for the Meridian Cloud API. Subscriptions are requested\n    from the Products page of the regional Meridian developer portal and activated on approval.\n  applies_to: Meridian Cloud API\n  docs: https://api-developer.meridiancloud.net/wiki/meridian/gettingstarted\n  method: searched\n- name: ems-platform-jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    EMS Platform Services requires a valid JWT authentication token on every API resource call.\n    Tokens are issued inside the customer tenancy; the legacy EMS SOAP API Web Service it replaces\n    authenticates with a predefined EMS user account instead.\n  applies_to: EMS Platform Services\n  docs: https://help.accruent.com/ems/Content/EMSPlatformServices/InstallationGuide/Introduction.html\n  method: searched\n\
  gaps:\n- The Maintenance Connection spec defines `basic` but applies it to zero of 255 operations.\n- No OAuth 2.0 or OpenID Connect anywhere in the published Accruent API surface.\n- No documented key rotation, expiry or scoping model for the Basic ConnectionKey/APIKey pair.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accruent/refs/heads/main/authentication/accruent-authentication.yml
summary_line: http/apiKey · 4 schemes
tags:
- Facilities Management
- Asset Management
- CMMS
- EAM
- Maintenance
- Work Orders
- IWMS
- Space Management
- Engineering Document Management
- Built Environment
- Enterprise Software
- Real Estate
---
