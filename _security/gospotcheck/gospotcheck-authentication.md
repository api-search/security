---
api_key_in: []
api_specs:
- filename: gospotcheck-asyncjobs-api-openapi.yml
  format: yaml
  label: GoSpotCheck AsyncJobs API
  slug: gospotcheck-asyncjobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-asyncjobs-api-openapi.yml
- filename: gospotcheck-catalogitems-api-openapi.yml
  format: yaml
  label: GoSpotCheck CatalogItems API
  slug: gospotcheck-catalogitems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-catalogitems-api-openapi.yml
- filename: gospotcheck-catalogs-api-openapi.yml
  format: yaml
  label: GoSpotCheck Catalogs API
  slug: gospotcheck-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-catalogs-api-openapi.yml
- filename: gospotcheck-customviews-api-openapi.yml
  format: yaml
  label: GoSpotCheck CustomViews API
  slug: gospotcheck-customviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-customviews-api-openapi.yml
- filename: gospotcheck-missionresponses-api-openapi.yml
  format: yaml
  label: GoSpotCheck MissionResponses API
  slug: gospotcheck-missionresponses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-missionresponses-api-openapi.yml
- filename: gospotcheck-missions-api-openapi.yml
  format: yaml
  label: GoSpotCheck Missions API
  slug: gospotcheck-missions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-missions-api-openapi.yml
- filename: gospotcheck-placegroups-api-openapi.yml
  format: yaml
  label: GoSpotCheck PlaceGroups API
  slug: gospotcheck-placegroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-placegroups-api-openapi.yml
- filename: gospotcheck-places-api-openapi.yml
  format: yaml
  label: GoSpotCheck Places API
  slug: gospotcheck-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-places-api-openapi.yml
- filename: gospotcheck-taskresponses-api-openapi.yml
  format: yaml
  label: GoSpotCheck TaskResponses API
  slug: gospotcheck-taskresponses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-taskresponses-api-openapi.yml
- filename: gospotcheck-tasks-api-openapi.yml
  format: yaml
  label: GoSpotCheck Tasks API
  slug: gospotcheck-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-tasks-api-openapi.yml
- filename: gospotcheck-teams-api-openapi.yml
  format: yaml
  label: GoSpotCheck Teams API
  slug: gospotcheck-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-teams-api-openapi.yml
- filename: gospotcheck-userplaceassignments-api-openapi.yml
  format: yaml
  label: GoSpotCheck UserPlaceAssignments API
  slug: gospotcheck-userplaceassignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-userplaceassignments-api-openapi.yml
- filename: gospotcheck-users-api-openapi.yml
  format: yaml
  label: GoSpotCheck Users API
  slug: gospotcheck-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gospotcheck Authentication
name_suffix: Authentication
oauth_flows: []
overview: GoSpotCheck secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GoSpotCheck
provider_slug: gospotcheck
scheme_count: 1
schemes:
- description: 'OAuth2 access token supplied as `Authorization: Bearer <token>`. Tokens are issued by GoSpotCheck; contact your Customer Success Manager or support@gospotcheck.com to obtain one.'
  name: oauth2Bearer
  scheme: bearer
  sources:
  - openapi/gospotcheck-external-openapi.yml
  type: http
slug: gospotcheck-authentication
source_filename: gospotcheck-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/gospotcheck-external-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: oauth2Bearer\n  type: http\n  scheme: bearer\n  description: 'OAuth2 access token supplied as `Authorization: Bearer <token>`. Tokens are\n    issued by GoSpotCheck; contact your Customer Success Manager or support@gospotcheck.com\n    to obtain one.'\n  sources:\n  - openapi/gospotcheck-external-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/authentication/gospotcheck-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Retail Execution
- Field Service
- Data Collection
- Surveys
- Merchandising
- CPG
- Mobile
---
