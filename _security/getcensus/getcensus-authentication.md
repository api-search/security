---
api_key_in: []
api_specs:
- filename: overview
  format: yaml
  label: Census Management API
  slug: census-management-api
  spec_type: Postman
  url: https://www.postman.com/getcensus/workspace/census-api/overview
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Getcensus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Census secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Census
provider_slug: getcensus
scheme_count: 2
schemes:
- applies_to: Workspace APIs
  description: Workspace-scoped operations (syncs, sync runs, sources, models, topics, tables, destinations, destination objects, destination types, connect links, webhooks) are authenticated with a workspace API key presented as an HTTP Bearer token.
  header: 'Authorization: Bearer <workspace-access-token>'
  name: workspaceBearerAuth
  provisioning: Open the workspace, then Workspace settings -> "API Access" to retrieve the workspace API key.
  scheme: bearer
  sources:
  - https://fivetran.com/docs/activations/rest-api/api-reference/introduction/authorization.md
  type: http
- applies_to: Organization APIs
  description: Organization-scoped operations (workspaces, workspace users, workspace variables, users, invitations) are authenticated with a Personal Access Token presented as an HTTP Bearer token. A PAT carries the same permissions as the user who generated it, so admin operations such as creating and managing workspaces require an admin user.
  header: 'Authorization: Bearer <personal-access-token>'
  name: organizationBearerAuth
  provisioning: User settings page (https://fivetran.com/dashboard/activations/home/user-settings) -> "Personal Access Tokens" -> New Token.
  scheme: bearer
  sources:
  - https://fivetran.com/docs/activations/rest-api/api-reference/introduction/authorization.md
  type: http
slug: getcensus-authentication
source_filename: getcensus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://fivetran.com/docs/activations/rest-api/api-reference/introduction/authorization.md\ndocs: https://fivetran.com/docs/activations/rest-api/api-reference/introduction/authorization\nnote: >-\n  Census now ships as Fivetran Activations; the Census Management API reference moved from\n  developers.getcensus.com (which 301s to fivetran.com/docs/activations/rest-api) onto the Fivetran\n  docs host, but the API itself is still served from app.getcensus.com / app-eu.getcensus.com and is\n  still authenticated with Census-issued Bearer tokens. Derived mechanically was not possible: the\n  provider publishes no OpenAPI for this API (see conformance/ and the x-coverage block in apis.yml),\n  so this profile was read from the published authentication page rather than from securitySchemes.\nsummary:\n  types:\n    - http\n  http_schemes:\n    - bearer\n  api_key_in: []\n  oauth2_flows: []\n  token_kinds:\n    - workspace-api-key\n\
  \    - personal-access-token\nschemes:\n  - name: workspaceBearerAuth\n    type: http\n    scheme: bearer\n    applies_to: Workspace APIs\n    description: >-\n      Workspace-scoped operations (syncs, sync runs, sources, models, topics, tables, destinations,\n      destination objects, destination types, connect links, webhooks) are authenticated with a\n      workspace API key presented as an HTTP Bearer token.\n    header: 'Authorization: Bearer <workspace-access-token>'\n    provisioning: >-\n      Open the workspace, then Workspace settings -> \"API Access\" to retrieve the workspace API key.\n    sources:\n      - https://fivetran.com/docs/activations/rest-api/api-reference/introduction/authorization.md\n  - name: organizationBearerAuth\n    type: http\n    scheme: bearer\n    applies_to: Organization APIs\n    description: >-\n      Organization-scoped operations (workspaces, workspace users, workspace variables, users,\n      invitations) are authenticated with a Personal Access\
  \ Token presented as an HTTP Bearer token.\n      A PAT carries the same permissions as the user who generated it, so admin operations such as\n      creating and managing workspaces require an admin user.\n    header: 'Authorization: Bearer <personal-access-token>'\n    provisioning: >-\n      User settings page (https://fivetran.com/dashboard/activations/home/user-settings) ->\n      \"Personal Access Tokens\" -> New Token.\n    sources:\n      - https://fivetran.com/docs/activations/rest-api/api-reference/introduction/authorization.md\nregions:\n  - name: US\n    base_url: https://app.getcensus.com\n    example: https://app.getcensus.com/api/v1/syncs\n  - name: EU\n    base_url: https://app-eu.getcensus.com\n    example: https://app-eu.getcensus.com/api/v1/syncs\nguidance:\n  - Tokens must never be embedded in client-side code or committed to a repository.\n  - A compromised token is regenerated or deleted from Fivetran Activations settings.\n  - >-\n    The Terraform provider reads\
  \ the organization Personal Access Token from the\n    CENSUS_PERSONAL_ACCESS_TOKEN environment variable and takes a region argument (us | eu | au).\ntransition:\n  note: >-\n    The Users and Invitations organization endpoints were deprecated on 2026-05-01 and are replaced\n    by Fivetran's own Users endpoints, which use Fivetran's standard auth mechanism rather than the\n    Activations workspace/personal token. Fivetran advises developers to run both key types in\n    parallel during the migration.\n  source: https://whatsnew.getcensus.com/activations-user-list-and-invitation-apis-deprecated-336835\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getcensus/refs/heads/main/authentication/getcensus-authentication.yml
summary_line: http · 2 schemes
tags:
- Reverse ETL
- Data Activation
- Data Warehouse
- CRM
- Marketing Automation
- Segments
- Syncs
- SQL
---
