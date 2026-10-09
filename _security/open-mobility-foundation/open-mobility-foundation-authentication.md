---
anonymous_access: false
api_key_in: []
api_specs:
- filename: open-mobility-foundation-events-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Events API
  slug: open-mobility-foundation-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-events-api-openapi.yml
- filename: open-mobility-foundation-geographies-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Geographies API
  slug: open-mobility-foundation-geographies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-geographies-api-openapi.yml
- filename: open-mobility-foundation-geographies-json-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Geographies.json API
  slug: open-mobility-foundation-geographies-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-geographies-json-api-openapi.yml
- filename: open-mobility-foundation-jurisdictions-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Jurisdictions API
  slug: open-mobility-foundation-jurisdictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-jurisdictions-api-openapi.yml
- filename: open-mobility-foundation-jurisdictions-json-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Jurisdictions.json API
  slug: open-mobility-foundation-jurisdictions-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-jurisdictions-json-api-openapi.yml
- filename: open-mobility-foundation-metrics-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Metrics API
  slug: open-mobility-foundation-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-metrics-api-openapi.yml
- filename: open-mobility-foundation-policies-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Policies API
  slug: open-mobility-foundation-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-policies-api-openapi.yml
- filename: open-mobility-foundation-policies-json-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Policies.json API
  slug: open-mobility-foundation-policies-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-policies-json-api-openapi.yml
- filename: open-mobility-foundation-reports-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Reports API
  slug: open-mobility-foundation-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-reports-api-openapi.yml
- filename: open-mobility-foundation-requirements-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Requirements API
  slug: open-mobility-foundation-requirements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-requirements-api-openapi.yml
- filename: open-mobility-foundation-stops-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Stops API
  slug: open-mobility-foundation-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-stops-api-openapi.yml
- filename: open-mobility-foundation-telemetry-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Telemetry API
  slug: open-mobility-foundation-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-telemetry-api-openapi.yml
- filename: open-mobility-foundation-trips-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Trips API
  slug: open-mobility-foundation-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-trips-api-openapi.yml
- filename: open-mobility-foundation-value-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Value API
  slug: open-mobility-foundation-value-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-value-api-openapi.yml
- filename: open-mobility-foundation-vehicles-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Vehicles API
  slug: open-mobility-foundation-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-vehicles-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Open Mobility Foundation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Open Mobility Foundation secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Open Mobility Foundation
provider_slug: open-mobility-foundation
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'All MDS Agency endpoints require authentication.


    JSON Web Token ([JWT](https://jwt.io/introduction/)) is RECOMMENDED as the token format.


    When making requests, the endpoints expect `provider_id` to be part of the claims the JWT. The token issuance,

    expiration and revocation policies are at the discretion of the agency.'
  name: bearer
  scheme: bearer
  sources:
  - openapi/open-mobility-foundation-mds-agency-openapi.yml
  - openapi/open-mobility-foundation-mds-metrics-openapi.yml
  - openapi/open-mobility-foundation-mds-provider-openapi.yml
  type: http
slug: open-mobility-foundation-authentication
source_filename: open-mobility-foundation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: searched\nsource: https://github.com/openmobilityfoundation/mobility-data-specification/blob/main/general-information.md#authorization\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'All MDS Agency endpoints require authentication.\n\n\n    JSON Web Token ([JWT](https://jwt.io/introduction/)) is RECOMMENDED as the token format.\n\n\n    When making requests, the endpoints expect `provider_id` to be part of the claims the JWT. The token issuance,\n\n    expiration and revocation policies are at the discretion of the agency.'\n  sources:\n  - openapi/open-mobility-foundation-mds-agency-openapi.yml\n  - openapi/open-mobility-foundation-mds-metrics-openapi.yml\n  - openapi/open-mobility-foundation-mds-provider-openapi.yml\ndocs: https://github.com/openmobilityfoundation/mobility-data-specification/blob/main/general-information.md#authorization\nnotes:\n- All MDS Provider,\
  \ Agency, and Metrics APIs require authentication; Policy, Geography and Jurisdiction APIs must\n  be unauthenticated and public (per General Information).\n- Authorization header carries \"Bearer <token>\"; JWT (RFC 7519) is RECOMMENDED as the token format.\n- OAuth 2.0's client_credentials grant type (RFC 6749 section 4.4) is RECOMMENDED as the authentication and authorization\n  scheme; producers MAY define token scopes.\n- 'MDS is a specification with no fixed server: each regulatory agency or mobility provider hosts its own implementation\n  and issues its own tokens.'\npublic_apis:\n- policy\n- geography\n- jurisdiction\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/authentication/open-mobility-foundation-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Mobility
- Open Source
- Open Standards
- Transportation
- Cities
- Micromobility
- Data Specifications
---
