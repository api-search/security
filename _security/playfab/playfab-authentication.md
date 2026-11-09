---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: playfab-client-openapi.yml
  format: yaml
  label: PlayFab Client API
  slug: playfab-client-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-client-openapi.yml
- filename: playfab-server-openapi.yml
  format: yaml
  label: PlayFab Server API
  slug: playfab-server-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-server-openapi.yml
- filename: playfab-admin-openapi.yml
  format: yaml
  label: PlayFab Admin API
  slug: playfab-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-admin-openapi.yml
- filename: playfab-authentication-openapi.yml
  format: yaml
  label: PlayFab Authentication API
  slug: playfab-entity-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-authentication-openapi.yml
- filename: playfab-cloudscript-openapi.yml
  format: yaml
  label: PlayFab CloudScript API
  slug: playfab-cloudscript-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-cloudscript-openapi.yml
- filename: playfab-multiplayer-openapi.yml
  format: yaml
  label: PlayFab Multiplayer API
  slug: playfab-multiplayer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-multiplayer-openapi.yml
- filename: playfab-economy-openapi.yml
  format: yaml
  label: PlayFab Economy (Catalog / Inventory) API
  slug: playfab-economy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-economy-openapi.yml
- filename: playfab-data-openapi.yml
  format: yaml
  label: PlayFab Data API
  slug: playfab-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-data-openapi.yml
- filename: playfab-groups-openapi.yml
  format: yaml
  label: PlayFab Groups API
  slug: playfab-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-groups-openapi.yml
- filename: playfab-profiles-openapi.yml
  format: yaml
  label: PlayFab Profiles API
  slug: playfab-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-profiles-openapi.yml
- filename: playfab-events-openapi.yml
  format: yaml
  label: PlayFab Events API
  slug: playfab-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-events-openapi.yml
- filename: playfab-insights-openapi.yml
  format: yaml
  label: PlayFab Insights API
  slug: playfab-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-insights-openapi.yml
- filename: playfab-localization-openapi.yml
  format: yaml
  label: PlayFab Localization API
  slug: playfab-localization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-localization-openapi.yml
- filename: playfab-addon-openapi.yml
  format: yaml
  label: PlayFab Addon API
  slug: playfab-addon-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-addon-openapi.yml
- filename: playfab-experimentation-openapi.yml
  format: yaml
  label: PlayFab Experimentation API
  slug: playfab-experimentation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-experimentation-openapi.yml
- filename: playfab-leaderboards-openapi.yml
  format: yaml
  label: PlayFab Leaderboards API
  slug: playfab-leaderboards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-leaderboards-openapi.yml
- filename: playfab-progression-openapi.yml
  format: yaml
  label: PlayFab Progression API
  slug: playfab-progression-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-progression-openapi.yml
- filename: playfab-account-api-openapi.yml
  format: yaml
  label: PlayFab Account API
  slug: playfab-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-account-api-openapi.yml
- filename: playfab-authentication-api-openapi.yml
  format: yaml
  label: PlayFab Authentication API
  slug: playfab-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-authentication-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: derived
name: Playfab Authentication
name_suffix: Authentication
oauth_flows: []
overview: PlayFab secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PlayFab
provider_slug: playfab
scheme_count: 4
schemes:
- description: 'Session ticket returned by a successful `LoginWith*` call. Required

    for all Client API operations other than login/registration.'
  in: header
  name: sessionTicket
  parameter: X-Authorization
  sources:
  - openapi/playfab-account-api-openapi.yml
  - openapi/playfab-addon-openapi.yml
  - openapi/playfab-admin-openapi.yml
  - openapi/playfab-authentication-api-openapi.yml
  - openapi/playfab-authentication-openapi.yml
  - openapi/playfab-client-openapi.yml
  - openapi/playfab-cloudscript-openapi.yml
  - openapi/playfab-data-openapi.yml
  - openapi/playfab-economy-openapi.yml
  - openapi/playfab-events-openapi.yml
  - openapi/playfab-experimentation-openapi.yml
  - openapi/playfab-groups-openapi.yml
  - openapi/playfab-insights-openapi.yml
  - openapi/playfab-leaderboards-openapi.yml
  - openapi/playfab-localization-openapi.yml
  - openapi/playfab-multiplayer-openapi.yml
  - openapi/playfab-profiles-openapi.yml
  - openapi/playfab-progression-openapi.yml
  - openapi/playfab-server-openapi.yml
  type: apiKey
- description: Entity token used for Entity-model API calls.
  in: header
  name: entityToken
  parameter: X-EntityToken
  sources:
  - openapi/playfab-account-api-openapi.yml
  - openapi/playfab-addon-openapi.yml
  - openapi/playfab-admin-openapi.yml
  - openapi/playfab-authentication-api-openapi.yml
  - openapi/playfab-authentication-openapi.yml
  - openapi/playfab-client-openapi.yml
  - openapi/playfab-cloudscript-openapi.yml
  - openapi/playfab-data-openapi.yml
  - openapi/playfab-economy-openapi.yml
  - openapi/playfab-events-openapi.yml
  - openapi/playfab-experimentation-openapi.yml
  - openapi/playfab-groups-openapi.yml
  - openapi/playfab-insights-openapi.yml
  - openapi/playfab-leaderboards-openapi.yml
  - openapi/playfab-localization-openapi.yml
  - openapi/playfab-multiplayer-openapi.yml
  - openapi/playfab-profiles-openapi.yml
  - openapi/playfab-progression-openapi.yml
  - openapi/playfab-server-openapi.yml
  type: apiKey
- description: This API requires no authentication headers (usually provides one to other calls).
  in: header
  name: None
  parameter: None
  sources:
  - openapi/playfab-addon-openapi.yml
  - openapi/playfab-admin-openapi.yml
  - openapi/playfab-authentication-openapi.yml
  - openapi/playfab-client-openapi.yml
  - openapi/playfab-cloudscript-openapi.yml
  - openapi/playfab-data-openapi.yml
  - openapi/playfab-economy-openapi.yml
  - openapi/playfab-events-openapi.yml
  - openapi/playfab-experimentation-openapi.yml
  - openapi/playfab-groups-openapi.yml
  - openapi/playfab-insights-openapi.yml
  - openapi/playfab-leaderboards-openapi.yml
  - openapi/playfab-localization-openapi.yml
  - openapi/playfab-multiplayer-openapi.yml
  - openapi/playfab-profiles-openapi.yml
  - openapi/playfab-progression-openapi.yml
  - openapi/playfab-server-openapi.yml
  type: apiKey
- description: This API requires a title secret key, available to title admins, from PlayFab Game Manager.
  in: header
  name: SecretKey
  parameter: X-SecretKey
  sources:
  - openapi/playfab-addon-openapi.yml
  - openapi/playfab-admin-openapi.yml
  - openapi/playfab-authentication-openapi.yml
  - openapi/playfab-client-openapi.yml
  - openapi/playfab-cloudscript-openapi.yml
  - openapi/playfab-data-openapi.yml
  - openapi/playfab-economy-openapi.yml
  - openapi/playfab-events-openapi.yml
  - openapi/playfab-experimentation-openapi.yml
  - openapi/playfab-groups-openapi.yml
  - openapi/playfab-insights-openapi.yml
  - openapi/playfab-leaderboards-openapi.yml
  - openapi/playfab-localization-openapi.yml
  - openapi/playfab-multiplayer-openapi.yml
  - openapi/playfab-profiles-openapi.yml
  - openapi/playfab-progression-openapi.yml
  - openapi/playfab-server-openapi.yml
  type: apiKey
slug: playfab-authentication
source_filename: playfab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/playfab-account-api-openapi.yml, openapi/playfab-addon-openapi.yml, openapi/playfab-admin-openapi.yml,\n  openapi/playfab-authentication-api-openapi.yml, openapi/playfab-authentication-openapi.yml,\n  openapi/playfab-client-openapi.yml, openapi/playfab-cloudscript-openapi.yml, openapi/playfab-data-openapi.yml,\n  openapi/playfab-economy-openapi.yml, openapi/playfab-events-openapi.yml, openapi/playfab-experimentation-openapi.yml,\n  openapi/playfab-groups-openapi.yml ...\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sessionTicket\n  type: apiKey\n  in: header\n  parameter: X-Authorization\n  description: |-\n    Session ticket returned by a successful `LoginWith*` call. Required\n    for all Client API operations other than login/registration.\n  sources:\n  - openapi/playfab-account-api-openapi.yml\n  - openapi/playfab-addon-openapi.yml\n  - openapi/playfab-admin-openapi.yml\n  - openapi/playfab-authentication-api-openapi.yml\n\
  \  - openapi/playfab-authentication-openapi.yml\n  - openapi/playfab-client-openapi.yml\n  - openapi/playfab-cloudscript-openapi.yml\n  - openapi/playfab-data-openapi.yml\n  - openapi/playfab-economy-openapi.yml\n  - openapi/playfab-events-openapi.yml\n  - openapi/playfab-experimentation-openapi.yml\n  - openapi/playfab-groups-openapi.yml\n  - openapi/playfab-insights-openapi.yml\n  - openapi/playfab-leaderboards-openapi.yml\n  - openapi/playfab-localization-openapi.yml\n  - openapi/playfab-multiplayer-openapi.yml\n  - openapi/playfab-profiles-openapi.yml\n  - openapi/playfab-progression-openapi.yml\n  - openapi/playfab-server-openapi.yml\n- name: entityToken\n  type: apiKey\n  in: header\n  parameter: X-EntityToken\n  description: Entity token used for Entity-model API calls.\n  sources:\n  - openapi/playfab-account-api-openapi.yml\n  - openapi/playfab-addon-openapi.yml\n  - openapi/playfab-admin-openapi.yml\n  - openapi/playfab-authentication-api-openapi.yml\n  - openapi/playfab-authentication-openapi.yml\n\
  \  - openapi/playfab-client-openapi.yml\n  - openapi/playfab-cloudscript-openapi.yml\n  - openapi/playfab-data-openapi.yml\n  - openapi/playfab-economy-openapi.yml\n  - openapi/playfab-events-openapi.yml\n  - openapi/playfab-experimentation-openapi.yml\n  - openapi/playfab-groups-openapi.yml\n  - openapi/playfab-insights-openapi.yml\n  - openapi/playfab-leaderboards-openapi.yml\n  - openapi/playfab-localization-openapi.yml\n  - openapi/playfab-multiplayer-openapi.yml\n  - openapi/playfab-profiles-openapi.yml\n  - openapi/playfab-progression-openapi.yml\n  - openapi/playfab-server-openapi.yml\n- name: None\n  type: apiKey\n  in: header\n  parameter: None\n  description: This API requires no authentication headers (usually provides one to other calls).\n  sources:\n  - openapi/playfab-addon-openapi.yml\n  - openapi/playfab-admin-openapi.yml\n  - openapi/playfab-authentication-openapi.yml\n  - openapi/playfab-client-openapi.yml\n  - openapi/playfab-cloudscript-openapi.yml\n  - openapi/playfab-data-openapi.yml\n\
  \  - openapi/playfab-economy-openapi.yml\n  - openapi/playfab-events-openapi.yml\n  - openapi/playfab-experimentation-openapi.yml\n  - openapi/playfab-groups-openapi.yml\n  - openapi/playfab-insights-openapi.yml\n  - openapi/playfab-leaderboards-openapi.yml\n  - openapi/playfab-localization-openapi.yml\n  - openapi/playfab-multiplayer-openapi.yml\n  - openapi/playfab-profiles-openapi.yml\n  - openapi/playfab-progression-openapi.yml\n  - openapi/playfab-server-openapi.yml\n- name: SecretKey\n  type: apiKey\n  in: header\n  parameter: X-SecretKey\n  description: This API requires a title secret key, available to title admins, from PlayFab\n    Game Manager.\n  sources:\n  - openapi/playfab-addon-openapi.yml\n  - openapi/playfab-admin-openapi.yml\n  - openapi/playfab-authentication-openapi.yml\n  - openapi/playfab-client-openapi.yml\n  - openapi/playfab-cloudscript-openapi.yml\n  - openapi/playfab-data-openapi.yml\n  - openapi/playfab-economy-openapi.yml\n  - openapi/playfab-events-openapi.yml\n\
  \  - openapi/playfab-experimentation-openapi.yml\n  - openapi/playfab-groups-openapi.yml\n  - openapi/playfab-insights-openapi.yml\n  - openapi/playfab-leaderboards-openapi.yml\n  - openapi/playfab-localization-openapi.yml\n  - openapi/playfab-multiplayer-openapi.yml\n  - openapi/playfab-profiles-openapi.yml\n  - openapi/playfab-progression-openapi.yml\n  - openapi/playfab-server-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/playfab/authentication/playfab-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Authentication
- Microsoft Azure
- Backend
- Backend-as-a-Service
- CloudScript
- Economy
- Game Backend
- Game Development
- Games
- Leaderboards
- Matchmaking
- Microsoft
- Multiplayer
- PlayFab
- REST
---
