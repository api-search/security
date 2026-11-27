---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: derived
name: Microsoft Xbox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft Xbox secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Microsoft Xbox
provider_slug: microsoft-xbox
scheme_count: 4
schemes:
- description: This API requires no authentication headers (usually provides one to other calls).
  in: header
  name: None
  parameter: None
  sources:
  - openapi/microsoft-xbox-playfab-addon-openapi.yml
  - openapi/microsoft-xbox-playfab-admin-openapi.yml
  - openapi/microsoft-xbox-playfab-authentication-openapi.yml
  - openapi/microsoft-xbox-playfab-client-openapi.yml
  - openapi/microsoft-xbox-playfab-cloudscript-openapi.yml
  - openapi/microsoft-xbox-playfab-data-openapi.yml
  - openapi/microsoft-xbox-playfab-economy-openapi.yml
  - openapi/microsoft-xbox-playfab-events-openapi.yml
  - openapi/microsoft-xbox-playfab-experimentation-openapi.yml
  - openapi/microsoft-xbox-playfab-groups-openapi.yml
  - openapi/microsoft-xbox-playfab-insights-openapi.yml
  - openapi/microsoft-xbox-playfab-leaderboards-openapi.yml
  - openapi/microsoft-xbox-playfab-localization-openapi.yml
  - openapi/microsoft-xbox-playfab-multiplayer-openapi.yml
  - openapi/microsoft-xbox-playfab-profiles-openapi.yml
  - openapi/microsoft-xbox-playfab-progression-openapi.yml
  - openapi/microsoft-xbox-playfab-server-openapi.yml
  type: apiKey
- description: This API requires a client session ticket, available from any Client Login function.
  in: header
  name: SessionTicket
  parameter: X-Authorization
  sources:
  - openapi/microsoft-xbox-playfab-addon-openapi.yml
  - openapi/microsoft-xbox-playfab-admin-openapi.yml
  - openapi/microsoft-xbox-playfab-authentication-openapi.yml
  - openapi/microsoft-xbox-playfab-client-openapi.yml
  - openapi/microsoft-xbox-playfab-cloudscript-openapi.yml
  - openapi/microsoft-xbox-playfab-data-openapi.yml
  - openapi/microsoft-xbox-playfab-economy-openapi.yml
  - openapi/microsoft-xbox-playfab-events-openapi.yml
  - openapi/microsoft-xbox-playfab-experimentation-openapi.yml
  - openapi/microsoft-xbox-playfab-groups-openapi.yml
  - openapi/microsoft-xbox-playfab-insights-openapi.yml
  - openapi/microsoft-xbox-playfab-leaderboards-openapi.yml
  - openapi/microsoft-xbox-playfab-localization-openapi.yml
  - openapi/microsoft-xbox-playfab-multiplayer-openapi.yml
  - openapi/microsoft-xbox-playfab-profiles-openapi.yml
  - openapi/microsoft-xbox-playfab-progression-openapi.yml
  - openapi/microsoft-xbox-playfab-server-openapi.yml
  type: apiKey
- description: This API requires a title secret key, available to title admins, from PlayFab Game Manager.
  in: header
  name: SecretKey
  parameter: X-SecretKey
  sources:
  - openapi/microsoft-xbox-playfab-addon-openapi.yml
  - openapi/microsoft-xbox-playfab-admin-openapi.yml
  - openapi/microsoft-xbox-playfab-authentication-openapi.yml
  - openapi/microsoft-xbox-playfab-client-openapi.yml
  - openapi/microsoft-xbox-playfab-cloudscript-openapi.yml
  - openapi/microsoft-xbox-playfab-data-openapi.yml
  - openapi/microsoft-xbox-playfab-economy-openapi.yml
  - openapi/microsoft-xbox-playfab-events-openapi.yml
  - openapi/microsoft-xbox-playfab-experimentation-openapi.yml
  - openapi/microsoft-xbox-playfab-groups-openapi.yml
  - openapi/microsoft-xbox-playfab-insights-openapi.yml
  - openapi/microsoft-xbox-playfab-leaderboards-openapi.yml
  - openapi/microsoft-xbox-playfab-localization-openapi.yml
  - openapi/microsoft-xbox-playfab-multiplayer-openapi.yml
  - openapi/microsoft-xbox-playfab-profiles-openapi.yml
  - openapi/microsoft-xbox-playfab-progression-openapi.yml
  - openapi/microsoft-xbox-playfab-server-openapi.yml
  type: apiKey
- description: This API requires an Entity Session Token, available from the Entity GetEntityToken method.
  in: header
  name: EntityToken
  parameter: X-EntityToken
  sources:
  - openapi/microsoft-xbox-playfab-addon-openapi.yml
  - openapi/microsoft-xbox-playfab-admin-openapi.yml
  - openapi/microsoft-xbox-playfab-authentication-openapi.yml
  - openapi/microsoft-xbox-playfab-client-openapi.yml
  - openapi/microsoft-xbox-playfab-cloudscript-openapi.yml
  - openapi/microsoft-xbox-playfab-data-openapi.yml
  - openapi/microsoft-xbox-playfab-economy-openapi.yml
  - openapi/microsoft-xbox-playfab-events-openapi.yml
  - openapi/microsoft-xbox-playfab-experimentation-openapi.yml
  - openapi/microsoft-xbox-playfab-groups-openapi.yml
  - openapi/microsoft-xbox-playfab-insights-openapi.yml
  - openapi/microsoft-xbox-playfab-leaderboards-openapi.yml
  - openapi/microsoft-xbox-playfab-localization-openapi.yml
  - openapi/microsoft-xbox-playfab-multiplayer-openapi.yml
  - openapi/microsoft-xbox-playfab-profiles-openapi.yml
  - openapi/microsoft-xbox-playfab-progression-openapi.yml
  - openapi/microsoft-xbox-playfab-server-openapi.yml
  type: apiKey
slug: microsoft-xbox-authentication
source_filename: microsoft-xbox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/microsoft-xbox-playfab-addon-openapi.yml, openapi/microsoft-xbox-playfab-admin-openapi.yml,\n  openapi/microsoft-xbox-playfab-authentication-openapi.yml, openapi/microsoft-xbox-playfab-client-openapi.yml,\n  openapi/microsoft-xbox-playfab-cloudscript-openapi.yml, openapi/microsoft-xbox-playfab-data-openapi.yml,\n  openapi/microsoft-xbox-playfab-economy-openapi.yml, openapi/microsoft-xbox-playfab-events-openapi.yml,\n  openapi/microsoft-xbox-playfab-experimentation-openapi.yml, openapi/microsoft-xbox-playfab-groups-openapi.yml,\n  openapi/microsoft-xbox-playfab-insights-openapi.yml, openapi/microsoft-xbox-playfab-leaderboards-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: None\n  type: apiKey\n  in: header\n  parameter: None\n  description: This API requires no authentication headers (usually provides one to other calls).\n  sources:\n  - openapi/microsoft-xbox-playfab-addon-openapi.yml\n\
  \  - openapi/microsoft-xbox-playfab-admin-openapi.yml\n  - openapi/microsoft-xbox-playfab-authentication-openapi.yml\n  - openapi/microsoft-xbox-playfab-client-openapi.yml\n  - openapi/microsoft-xbox-playfab-cloudscript-openapi.yml\n  - openapi/microsoft-xbox-playfab-data-openapi.yml\n  - openapi/microsoft-xbox-playfab-economy-openapi.yml\n  - openapi/microsoft-xbox-playfab-events-openapi.yml\n  - openapi/microsoft-xbox-playfab-experimentation-openapi.yml\n  - openapi/microsoft-xbox-playfab-groups-openapi.yml\n  - openapi/microsoft-xbox-playfab-insights-openapi.yml\n  - openapi/microsoft-xbox-playfab-leaderboards-openapi.yml\n  - openapi/microsoft-xbox-playfab-localization-openapi.yml\n  - openapi/microsoft-xbox-playfab-multiplayer-openapi.yml\n  - openapi/microsoft-xbox-playfab-profiles-openapi.yml\n  - openapi/microsoft-xbox-playfab-progression-openapi.yml\n  - openapi/microsoft-xbox-playfab-server-openapi.yml\n- name: SessionTicket\n  type: apiKey\n  in: header\n  parameter: X-Authorization\n\
  \  description: This API requires a client session ticket, available from any Client Login function.\n  sources:\n  - openapi/microsoft-xbox-playfab-addon-openapi.yml\n  - openapi/microsoft-xbox-playfab-admin-openapi.yml\n  - openapi/microsoft-xbox-playfab-authentication-openapi.yml\n  - openapi/microsoft-xbox-playfab-client-openapi.yml\n  - openapi/microsoft-xbox-playfab-cloudscript-openapi.yml\n  - openapi/microsoft-xbox-playfab-data-openapi.yml\n  - openapi/microsoft-xbox-playfab-economy-openapi.yml\n  - openapi/microsoft-xbox-playfab-events-openapi.yml\n  - openapi/microsoft-xbox-playfab-experimentation-openapi.yml\n  - openapi/microsoft-xbox-playfab-groups-openapi.yml\n  - openapi/microsoft-xbox-playfab-insights-openapi.yml\n  - openapi/microsoft-xbox-playfab-leaderboards-openapi.yml\n  - openapi/microsoft-xbox-playfab-localization-openapi.yml\n  - openapi/microsoft-xbox-playfab-multiplayer-openapi.yml\n  - openapi/microsoft-xbox-playfab-profiles-openapi.yml\n  - openapi/microsoft-xbox-playfab-progression-openapi.yml\n\
  \  - openapi/microsoft-xbox-playfab-server-openapi.yml\n- name: SecretKey\n  type: apiKey\n  in: header\n  parameter: X-SecretKey\n  description: This API requires a title secret key, available to title admins, from PlayFab\n    Game Manager.\n  sources:\n  - openapi/microsoft-xbox-playfab-addon-openapi.yml\n  - openapi/microsoft-xbox-playfab-admin-openapi.yml\n  - openapi/microsoft-xbox-playfab-authentication-openapi.yml\n  - openapi/microsoft-xbox-playfab-client-openapi.yml\n  - openapi/microsoft-xbox-playfab-cloudscript-openapi.yml\n  - openapi/microsoft-xbox-playfab-data-openapi.yml\n  - openapi/microsoft-xbox-playfab-economy-openapi.yml\n  - openapi/microsoft-xbox-playfab-events-openapi.yml\n  - openapi/microsoft-xbox-playfab-experimentation-openapi.yml\n  - openapi/microsoft-xbox-playfab-groups-openapi.yml\n  - openapi/microsoft-xbox-playfab-insights-openapi.yml\n  - openapi/microsoft-xbox-playfab-leaderboards-openapi.yml\n  - openapi/microsoft-xbox-playfab-localization-openapi.yml\n\
  \  - openapi/microsoft-xbox-playfab-multiplayer-openapi.yml\n  - openapi/microsoft-xbox-playfab-profiles-openapi.yml\n  - openapi/microsoft-xbox-playfab-progression-openapi.yml\n  - openapi/microsoft-xbox-playfab-server-openapi.yml\n- name: EntityToken\n  type: apiKey\n  in: header\n  parameter: X-EntityToken\n  description: This API requires an Entity Session Token, available from the Entity GetEntityToken\n    method.\n  sources:\n  - openapi/microsoft-xbox-playfab-addon-openapi.yml\n  - openapi/microsoft-xbox-playfab-admin-openapi.yml\n  - openapi/microsoft-xbox-playfab-authentication-openapi.yml\n  - openapi/microsoft-xbox-playfab-client-openapi.yml\n  - openapi/microsoft-xbox-playfab-cloudscript-openapi.yml\n  - openapi/microsoft-xbox-playfab-data-openapi.yml\n  - openapi/microsoft-xbox-playfab-economy-openapi.yml\n  - openapi/microsoft-xbox-playfab-events-openapi.yml\n  - openapi/microsoft-xbox-playfab-experimentation-openapi.yml\n  - openapi/microsoft-xbox-playfab-groups-openapi.yml\n\
  \  - openapi/microsoft-xbox-playfab-insights-openapi.yml\n  - openapi/microsoft-xbox-playfab-leaderboards-openapi.yml\n  - openapi/microsoft-xbox-playfab-localization-openapi.yml\n  - openapi/microsoft-xbox-playfab-multiplayer-openapi.yml\n  - openapi/microsoft-xbox-playfab-profiles-openapi.yml\n  - openapi/microsoft-xbox-playfab-progression-openapi.yml\n  - openapi/microsoft-xbox-playfab-server-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-xbox/authentication/microsoft-xbox-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Gaming
- Microsoft
- PlayFab
- Xbox
- Xbox Live
- Video Games
---
