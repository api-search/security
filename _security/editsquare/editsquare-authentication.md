---
anonymous_access: false
api_key_in: []
api_specs:
- filename: editsquare-projects-api-openapi.yml
  format: yaml
  label: Edit Square Projects API
  slug: editsquare-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/editsquare/refs/heads/main/openapi/editsquare-projects-api-openapi.yml
- filename: editsquare-renders-api-openapi.yml
  format: yaml
  label: Edit Square Renders API
  slug: editsquare-renders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/editsquare/refs/heads/main/openapi/editsquare-renders-api-openapi.yml
- filename: editsquare-teams-api-openapi.yml
  format: yaml
  label: Edit Square Teams API
  slug: editsquare-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/editsquare/refs/heads/main/openapi/editsquare-teams-api-openapi.yml
- filename: editsquare-templates-api-openapi.yml
  format: yaml
  label: Edit Square Templates API
  slug: editsquare-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/editsquare/refs/heads/main/openapi/editsquare-templates-api-openapi.yml
- filename: editsquare-users-api-openapi.yml
  format: yaml
  label: Edit Square Users API
  slug: editsquare-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/editsquare/refs/heads/main/openapi/editsquare-users-api-openapi.yml
auth_types: []
description: 'All Edit Square endpoints are authenticated using API keys as a bearer token:'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Editsquare Authentication
name_suffix: Authentication
oauth_flows: []
overview: Edit Square declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Edit Square
provider_slug: editsquare
scheme_count: 1
schemes:
- evidence: 'All Edit Square endpoints are authenticated using API keys as a bearer token:'
  header: Authorization
  how_to_obtain: 'Keys are created in the dashboard: open the dashboard, click your avatar, choose API Keys, create a key and give it a name.'
  location: header
  name: Bearer
  type: http-bearer
slug: editsquare-authentication
source_filename: editsquare-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.editsquare.com/api/authentication.md
source_yaml: "generated: '2026-10-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.editsquare.com/api/authentication.md\nsources:\n- https://docs.editsquare.com/api/authentication.md\ndescription: 'All Edit Square endpoints are authenticated using API keys as a bearer token:'\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'All Edit Square endpoints are authenticated using API keys as a bearer token:'\n  location: header\n  header: Authorization\n  how_to_obtain: 'Keys are created in the dashboard: open the dashboard, click your avatar, choose API Keys, create a key and give it a name.'\ndocs: https://docs.editsquare.com/api/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/editsquare/refs/heads/main/authentication/editsquare-authentication.yml
summary_line: 1 scheme
tags:
- Motion Graphics
- Video Editing
- Cloud Rendering
---
