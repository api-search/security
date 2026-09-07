---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: artemis-apod-api-openapi.yml
  format: yaml
  label: Artemis APOD API
  slug: artemis-apod-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artemis/refs/heads/main/openapi/artemis-apod-api-openapi.yml
- filename: artemis-donki-api-openapi.yml
  format: yaml
  label: Artemis DONKI API
  slug: artemis-donki-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artemis/refs/heads/main/openapi/artemis-donki-api-openapi.yml
- filename: artemis-epic-api-openapi.yml
  format: yaml
  label: Artemis EPIC API
  slug: artemis-epic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artemis/refs/heads/main/openapi/artemis-epic-api-openapi.yml
- filename: artemis-images-api-openapi.yml
  format: yaml
  label: Artemis Images API
  slug: artemis-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artemis/refs/heads/main/openapi/artemis-images-api-openapi.yml
- filename: artemis-neows-api-openapi.yml
  format: yaml
  label: Artemis NeoWs API
  slug: artemis-neows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artemis/refs/heads/main/openapi/artemis-neows-api-openapi.yml
- filename: artemis-techport-swagger.json
  format: json
  label: NASA TechPort API
  slug: nasa-techport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artemis/refs/heads/main/openapi/artemis-techport-swagger.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Artemis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Artemis secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Artemis
provider_slug: artemis
scheme_count: 1
schemes:
- description: A single api_key query parameter on every api.nasa.gov request. There is no header form documented and none was accepted on probe. DEMO_KEY is a published shared value for exploration.
  docs: https://api.nasa.gov/assets/html/authentication.html
  in: query
  name: NasaApiKey
  parameter: api_key
  required: true
  sources:
  - https://api.nasa.gov/assets/html/authentication.html
  - openapi/artemis-apod-swagger.json
  - openapi/artemis-apod-api-openapi.yml
  - openapi/artemis-donki-api-openapi.yml
  - openapi/artemis-epic-api-openapi.yml
  - openapi/artemis-images-api-openapi.yml
  - openapi/artemis-neows-api-openapi.yml
  type: apiKey
slug: artemis-authentication
source_filename: artemis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://api.nasa.gov/assets/html/authentication.html\ndocs:\n- https://api.nasa.gov/assets/html/authentication.html\n- https://api.data.gov/docs/developer-manual/\nnote: >-\n  Upgraded from derived to searched: NASA publishes a dedicated authentication page and it agrees\n  with the securitySchemes in the captured contracts. NASA's own Swagger for APOD\n  (openapi/artemis-apod-swagger.json, extracted from api.nasa.gov/assets/json/apis.json) declares\n  the same scheme, which makes this first-party rather than inferred.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  oauth2: false\n  oidc: false\n  mtls: false\n  anonymous_access: partial\nschemes:\n- name: NasaApiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  required: true\n  description: >-\n    A single api_key query parameter on every api.nasa.gov request. There is no header form\n    documented and none was accepted on probe. DEMO_KEY is a published\
  \ shared value for exploration.\n  docs: https://api.nasa.gov/assets/html/authentication.html\n  sources:\n  - https://api.nasa.gov/assets/html/authentication.html\n  - openapi/artemis-apod-swagger.json\n  - openapi/artemis-apod-api-openapi.yml\n  - openapi/artemis-donki-api-openapi.yml\n  - openapi/artemis-epic-api-openapi.yml\n  - openapi/artemis-images-api-openapi.yml\n  - openapi/artemis-neows-api-openapi.yml\nunauthenticated_surfaces:\n- host: images-api.nasa.gov\n  note: >-\n    The NASA Image and Video Library takes no key at all. Confirmed by live probe 2026-09-04 —\n    https://images-api.nasa.gov/search?q=artemis returned 200 with no credential.\n- host: trek.nasa.gov\n  note: Moon/Mars/Vesta Trek OGC WMTS tiles and Capabilities documents require no key.\n- host: gibs.earthdata.nasa.gov\n  note: NASA GIBS WMS/WMTS requires no key.\ncredential_issuance:\n  self_serve: true\n  signup_url: https://api.nasa.gov/#signUp\n  requires: name and email\n  approval: instant\n  recovery_url:\
  \ https://api.nasa.gov/assets/html/recoverKey.html\n  multiple_keys: true\n  note: >-\n    NASA states a key issued here \"can be used to access data across federal agencies\" — it is an\n    api.data.gov gateway credential, not a NASA-only one.\nrotation:\n  self_serve_rotation: false\n  expiry: none published\n  revocation: >-\n    Administrators can disable a key (error code API_KEY_DISABLED), but there is no self-serve\n    rotate or revoke surface documented.\nrisks:\n- id: key-in-query-string\n  severity: medium\n  detail: >-\n    The credential travels in the URL on every request, so it lands in server access logs, browser\n    history, proxy logs and Referer headers. The gateway also sets\n    `access-control-allow-origin: *`, which means browser clients call it directly and expose the key\n    client-side. Low blast radius here because the key grants read-only access to public data and\n    only gates rate limit — but it is the reason the Kin Score credentials_not_in_query check\
  \ fails\n    for every contract on this surface, and it is a real habit-forming problem for developers who\n    carry the pattern to APIs where it matters.\n- id: no-scopes\n  severity: low\n  detail: >-\n    One key, all APIs, no scope or permission model. There is nothing to least-privilege. See\n    scopes — none published, and none applicable without OAuth.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artemis/refs/heads/main/authentication/artemis-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Exploration
- Lunar
- Moon
- NASA
- Space
- Government
---
