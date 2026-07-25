---
api_key_in:
- header
api_specs:
- filename: prolific-aitaskbuilder-api-openapi.yml
  format: yaml
  label: Prolific aiTaskBuilder API
  slug: prolific-aitaskbuilder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific/refs/heads/main/openapi/prolific-aitaskbuilder-api-openapi.yml
- filename: prolific-bonuses-api-openapi.yml
  format: yaml
  label: Prolific bonuses API
  slug: prolific-bonuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific/refs/heads/main/openapi/prolific-bonuses-api-openapi.yml
- filename: prolific-credentials-api-openapi.yml
  format: yaml
  label: Prolific credentials API
  slug: prolific-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific/refs/heads/main/openapi/prolific-credentials-api-openapi.yml
- filename: prolific-filters-api-openapi.yml
  format: yaml
  label: Prolific filters API
  slug: prolific-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific/refs/heads/main/openapi/prolific-filters-api-openapi.yml
- filename: prolific-filtersets-api-openapi.yml
  format: yaml
  label: Prolific filterSets API
  slug: prolific-filtersets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific/refs/heads/main/openapi/prolific-filtersets-api-openapi.yml
- filename: prolific-invitations-api-openapi.yml
  format: yaml
  label: Prolific invitations API
  slug: prolific-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific/refs/heads/main/openapi/prolific-invitations-api-openapi.yml
- filename: prolific-messages-api-openapi.yml
  format: yaml
  label: Prolific messages API
  slug: prolific-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific/refs/heads/main/openapi/prolific-messages-api-openapi.yml
- filename: prolific-participantgroups-api-openapi.yml
  format: yaml
  label: Prolific participantGroups API
  slug: prolific-participantgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific/refs/heads/main/openapi/prolific-participantgroups-api-openapi.yml
- filename: prolific-projects-api-openapi.yml
  format: yaml
  label: Prolific projects API
  slug: prolific-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific/refs/heads/main/openapi/prolific-projects-api-openapi.yml
- filename: prolific-rewardrecommendations-api-openapi.yml
  format: yaml
  label: Prolific rewardRecommendations API
  slug: prolific-rewardrecommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific/refs/heads/main/openapi/prolific-rewardrecommendations-api-openapi.yml
- filename: prolific-studies-api-openapi.yml
  format: yaml
  label: Prolific studies API
  slug: prolific-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific/refs/heads/main/openapi/prolific-studies-api-openapi.yml
- filename: prolific-submissionfeedbackupload-api-openapi.yml
  format: yaml
  label: Prolific submissionFeedbackUpload API
  slug: prolific-submissionfeedbackupload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific/refs/heads/main/openapi/prolific-submissionfeedbackupload-api-openapi.yml
- filename: prolific-submissions-api-openapi.yml
  format: yaml
  label: Prolific submissions API
  slug: prolific-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific/refs/heads/main/openapi/prolific-submissions-api-openapi.yml
- filename: prolific-surveys-api-openapi.yml
  format: yaml
  label: Prolific surveys API
  slug: prolific-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific/refs/heads/main/openapi/prolific-surveys-api-openapi.yml
- filename: prolific-users-api-openapi.yml
  format: yaml
  label: Prolific users API
  slug: prolific-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific/refs/heads/main/openapi/prolific-users-api-openapi.yml
- filename: prolific-webhooks-api-openapi.yml
  format: yaml
  label: Prolific webhooks API
  slug: prolific-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific/refs/heads/main/openapi/prolific-webhooks-api-openapi.yml
- filename: prolific-wellknownendpoints-api-openapi.yml
  format: yaml
  label: Prolific wellKnownEndpoints API
  slug: prolific-wellknownendpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific/refs/heads/main/openapi/prolific-wellknownendpoints-api-openapi.yml
- filename: prolific-workspaces-api-openapi.yml
  format: yaml
  label: Prolific workspaces API
  slug: prolific-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific/refs/heads/main/openapi/prolific-workspaces-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Prolific Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prolific secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Prolific
provider_slug: prolific
scheme_count: 1
schemes:
- description: 'The Prolific API uses API token to authenticate requests. You can create an API token directly from your settings.


    Your API token does not have an expiry date and carries full permission, so be sure to keep them secure.


    If your token is leaked, delete it and create a new one directly in the app.


    In your requests add `Authorization` header with the value `Token <your token>`.'
  in: header
  name: token
  parameter: Authorization
  sources:
  - openapi/prolific-openapi-original.yml
  type: apiKey
slug: prolific-authentication
source_filename: prolific-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/prolific-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    The Prolific API uses API token to authenticate requests. You can create an API token directly from your settings.\n\n    Your API token does not have an expiry date and carries full permission, so be sure to keep them secure.\n\n    If your token is leaked, delete it and create a new one directly in the app.\n\n    In your requests add `Authorization` header with the value `Token <your token>`.\n  sources:\n  - openapi/prolific-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prolific/refs/heads/main/authentication/prolific-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ai/Ml
- Human Data
- Research
- Participant Recruitment
- Surveys
- Human Feedback
- RLHF
- Data Collection
- API
---
