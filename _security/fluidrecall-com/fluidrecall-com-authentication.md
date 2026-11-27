---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fluidrecall-com-accounts-api-openapi.yml
  format: yaml
  label: Fluid Recall Accounts API
  slug: fluidrecall-com-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluidrecall-com/openapi/fluidrecall-com-accounts-api-openapi.yml
- filename: fluidrecall-com-admin-api-openapi.yml
  format: yaml
  label: Fluid Recall Admin API
  slug: fluidrecall-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluidrecall-com/openapi/fluidrecall-com-admin-api-openapi.yml
- filename: fluidrecall-com-agent-api-openapi.yml
  format: yaml
  label: Fluid Recall Agent API
  slug: fluidrecall-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluidrecall-com/openapi/fluidrecall-com-agent-api-openapi.yml
- filename: fluidrecall-com-bootstrap-api-openapi.yml
  format: yaml
  label: Fluid Recall Bootstrap API
  slug: fluidrecall-com-bootstrap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluidrecall-com/openapi/fluidrecall-com-bootstrap-api-openapi.yml
- filename: fluidrecall-com-cards-api-openapi.yml
  format: yaml
  label: Fluid Recall Cards API
  slug: fluidrecall-com-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluidrecall-com/openapi/fluidrecall-com-cards-api-openapi.yml
- filename: fluidrecall-com-decks-api-openapi.yml
  format: yaml
  label: Fluid Recall Decks API
  slug: fluidrecall-com-decks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluidrecall-com/openapi/fluidrecall-com-decks-api-openapi.yml
- filename: fluidrecall-com-dev-api-openapi.yml
  format: yaml
  label: Fluid Recall Dev API
  slug: fluidrecall-com-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluidrecall-com/openapi/fluidrecall-com-dev-api-openapi.yml
- filename: fluidrecall-com-due-api-openapi.yml
  format: yaml
  label: Fluid Recall Due API
  slug: fluidrecall-com-due-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluidrecall-com/openapi/fluidrecall-com-due-api-openapi.yml
- filename: fluidrecall-com-export-api-openapi.yml
  format: yaml
  label: Fluid Recall Export API
  slug: fluidrecall-com-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluidrecall-com/openapi/fluidrecall-com-export-api-openapi.yml
- filename: fluidrecall-com-feedback-api-openapi.yml
  format: yaml
  label: Fluid Recall Feedback API
  slug: fluidrecall-com-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluidrecall-com/openapi/fluidrecall-com-feedback-api-openapi.yml
- filename: fluidrecall-com-mailboxes-api-openapi.yml
  format: yaml
  label: Fluid Recall Mailboxes API
  slug: fluidrecall-com-mailboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluidrecall-com/openapi/fluidrecall-com-mailboxes-api-openapi.yml
- filename: fluidrecall-com-messages-api-openapi.yml
  format: yaml
  label: Fluid Recall Messages API
  slug: fluidrecall-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluidrecall-com/openapi/fluidrecall-com-messages-api-openapi.yml
- filename: fluidrecall-com-plan-api-openapi.yml
  format: yaml
  label: Fluid Recall Plan API
  slug: fluidrecall-com-plan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluidrecall-com/openapi/fluidrecall-com-plan-api-openapi.yml
- filename: fluidrecall-com-reviews-api-openapi.yml
  format: yaml
  label: Fluid Recall Reviews API
  slug: fluidrecall-com-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluidrecall-com/openapi/fluidrecall-com-reviews-api-openapi.yml
- filename: fluidrecall-com-settings-api-openapi.yml
  format: yaml
  label: Fluid Recall Settings API
  slug: fluidrecall-com-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluidrecall-com/openapi/fluidrecall-com-settings-api-openapi.yml
- filename: fluidrecall-com-tokens-api-openapi.yml
  format: yaml
  label: Fluid Recall Tokens API
  slug: fluidrecall-com-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluidrecall-com/openapi/fluidrecall-com-tokens-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Fluid Recall Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fluid Recall secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Fluid Recall
provider_slug: fluidrecall-com
scheme_count: 2
schemes:
- description: Personal Fluid Recall API token from POST /accounts (or POST /bootstrap). Save it for API calls. The operator break-glass secret is a different credential and cannot call drill operations.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fluidrecall-com-openapi.json
  type: http
- description: 'Personal Agent Protocol (Poppy v0.1) Session Token from POST https://fluidrecall.com/oauth/token, sent as Authorization: DPoP <token> with a DPoP proof header on every call. poppy:read allows reads and poppy:write allows changes; personal API token management is not available. See https://fluidrecall.com/.well-known/poppy.json and https://fluidrecall.com/docs/personal-agent-protocol.'
  name: poppyDpop
  scheme: DPoP
  sources:
  - openapi/fluidrecall-com-openapi.json
  type: http
slug: fluidrecall-com-authentication
source_filename: fluidrecall-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/fluidrecall-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Personal Fluid Recall API token from POST /accounts (or POST /bootstrap). Save\n    it for API calls. The operator break-glass secret is a different credential and cannot call\n    drill operations.\n  sources:\n  - openapi/fluidrecall-com-openapi.json\n- name: poppyDpop\n  type: http\n  scheme: DPoP\n  description: 'Personal Agent Protocol (Poppy v0.1) Session Token from POST https://fluidrecall.com/oauth/token,\n    sent as Authorization: DPoP <token> with a DPoP proof header on every call. poppy:read allows\n    reads and poppy:write allows changes; personal API token management is not available. See\n    https://fluidrecall.com/.well-known/poppy.json and https://fluidrecall.com/docs/personal-agent-protocol.'\n  sources:\n  - openapi/fluidrecall-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/fluidrecall-com/authentication/fluidrecall-com-authentication.yml
summary_line: http · 2 schemes
tags:
- Artificial Intelligence
- Education
- Free
- OpenAPI
- Recall
---
