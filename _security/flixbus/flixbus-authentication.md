---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Flixbus Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: FlixBus secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: FlixBus
provider_slug: flixbus
scheme_count: 1
schemes:
- applies_to: https://global.api.flixbus.com/api
  flows:
  - client_id: 29f56109-061f-4497-adc6-a341b8da145c
    flow: authorizationCode
    library: MSAL (@azure/msal-browser)
    scope: api://5cd49e44-b725-40d7-949e-cfcd481d5201/user_impersonation
    tenant_id: d8d0ad3e-8bcf-48e9-9bb2-aee17c6c4fd5
  name: EntraID
  presentation: 'Authorization: Bearer <access_token>'
  provider: Microsoft Entra ID (Azure AD)
  sources:
  - https://developer.api.flixbus.com/static/js/main.66632736.js
  type: oauth2
slug: flixbus-authentication
source_filename: flixbus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: >-\n  https://developer.api.flixbus.com/static/js/main.66632736.js (portal runtime config)\n  and live anonymous probes of https://global.api.flixbus.com\ndocs: https://developer.api.flixbus.com/\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  spec_derived: false\n  note: >-\n    No OpenAPI is publicly reachable, so this profile is observed rather than derived\n    from securitySchemes. It describes the authentication the Flix Developer Portal\n    itself performs; the partner API's issued credentials are documented only behind\n    that login.\nschemes:\n- name: EntraID\n  type: oauth2\n  provider: Microsoft Entra ID (Azure AD)\n  flows:\n  - flow: authorizationCode\n    tenant_id: d8d0ad3e-8bcf-48e9-9bb2-aee17c6c4fd5\n    client_id: 29f56109-061f-4497-adc6-a341b8da145c\n    scope: api://5cd49e44-b725-40d7-949e-cfcd481d5201/user_impersonation\n    library: MSAL (@azure/msal-browser)\n\
  \  applies_to: https://global.api.flixbus.com/api\n  presentation: 'Authorization: Bearer <access_token>'\n  sources: ['https://developer.api.flixbus.com/static/js/main.66632736.js']\ngated:\n  portal: >-\n    developer.api.flixbus.com requires a Microsoft Entra ID sign-in before any API\n    reference, getting-started guide, changelog or Postman collection is visible.\n  gateway_observations:\n  - {url: 'https://global.api.flixbus.com/', http_status: 403}\n  - {url: 'https://global.api.flixbus.com/api/apis', http_status: 401, body: '{\"message\":\"Unauthorized\"}'}\n  - {url: 'https://global.api.flixbus.com/search/service/v4/search', http_status: 400}\nonboarding:\n  how_to_get_credentials: >-\n    Distribution / dynamic-integration access (API, GTFS, white label, metasearch) is\n    requested by emailing online-distribution@flixbus.com with company details, domains\n    and monthly visitor numbers. Static affiliate integration runs through AWIN.\n  contact: online-distribution@flixbus.com\n\
  \  url: https://global.flixbus.com/company/partners/affiliate-partners\nunauthenticated_surfaces:\n- name: GTFS Schedule feeds\n  auth: none\n  urls:\n  - https://gtfs.gis.flix.tech/gtfs_generic_eu.zip\n  - https://gtfs.gis.flix.tech/gtfs_generic_us.zip\n  - https://gtfs.gis.flix.tech/gtfs_generic_gb.zip\nx-evidence:\n  fetched: '2026-08-04'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flixbus/refs/heads/main/authentication/flixbus-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Transportation
- Travel
- Mobility
- Bus
- Rail
- Ticketing
- GTFS
- Open Data
- Distribution
---
