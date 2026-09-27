---
anonymous_access: false
api_key_in: []
api_specs:
- filename: axuall-actor-api-openapi.yml
  format: yaml
  label: Axuall Actor API
  slug: axuall-actor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-actor-api-openapi.yml
- filename: axuall-address-deduplications-api-openapi.yml
  format: yaml
  label: Axuall Address Deduplications API
  slug: axuall-address-deduplications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-address-deduplications-api-openapi.yml
- filename: axuall-agent-api-openapi.yml
  format: yaml
  label: Axuall Agent API
  slug: axuall-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-agent-api-openapi.yml
- filename: axuall-authentication-api-openapi.yml
  format: yaml
  label: Axuall Authentication API
  slug: axuall-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-authentication-api-openapi.yml
- filename: axuall-case-log-artifact-api-openapi.yml
  format: yaml
  label: Axuall Case Log Artifact API
  slug: axuall-case-log-artifact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-case-log-artifact-api-openapi.yml
- filename: axuall-documents-api-openapi.yml
  format: yaml
  label: Axuall Documents API
  slug: axuall-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-documents-api-openapi.yml
- filename: axuall-email-api-openapi.yml
  format: yaml
  label: Axuall Email API
  slug: axuall-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-email-api-openapi.yml
- filename: axuall-facilities-api-openapi.yml
  format: yaml
  label: Axuall Facilities API
  slug: axuall-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-facilities-api-openapi.yml
- filename: axuall-fsmb-artifact-api-openapi.yml
  format: yaml
  label: Axuall FSMB Artifact API
  slug: axuall-fsmb-artifact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-fsmb-artifact-api-openapi.yml
- filename: axuall-invite-api-openapi.yml
  format: yaml
  label: Axuall Invite API
  slug: axuall-invite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-invite-api-openapi.yml
- filename: axuall-monitoring-reports-api-openapi.yml
  format: yaml
  label: Axuall Monitoring reports API
  slug: axuall-monitoring-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-monitoring-reports-api-openapi.yml
- filename: axuall-provider-preview-api-openapi.yml
  format: yaml
  label: Axuall Provider Preview API
  slug: axuall-provider-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-provider-preview-api-openapi.yml
- filename: axuall-providers-api-openapi.yml
  format: yaml
  label: Axuall Providers API
  slug: axuall-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-providers-api-openapi.yml
- filename: axuall-recipes-api-openapi.yml
  format: yaml
  label: Axuall Recipes API
  slug: axuall-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-recipes-api-openapi.yml
- filename: axuall-tasks-api-openapi.yml
  format: yaml
  label: Axuall Tasks API
  slug: axuall-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-tasks-api-openapi.yml
auth_types: []
description: Authentication schemes for Axuall API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Axuall Authentication
name_suffix: Authentication
oauth_flows: []
overview: Axuall declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Axuall
provider_slug: axuall
scheme_count: 1
schemes:
- evidence: The Axuall API uses Auth0 to authenticate all API clients.
  flows:
  - client_credentials
  how_to_obtain: Send a POST request to the token URL with client_id and client_secret in the JSON body.
  name: Auth0
  token_url: https://api.axuall.net/v2/auth
  type: oauth2
slug: axuall-authentication
source_filename: axuall-authentication.yml
source_heading: Authentication Profile
source_url: https://axuall.readme.io/reference/authenticate_user_v2_auth_post
source_yaml: "generated: '2026-09-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://axuall.readme.io/reference/authenticate_user_v2_auth_post\nsources:\n- https://axuall.readme.io/reference/authenticate_user_v2_auth_post\n- https://docs.readme.com/main/docs/oauth-workflows-in-try-it\n- https://docs.readme.com/main/docs/two-factor-authentication\n- https://axuall.readme.io/reference/authenticate_user_v2_auth_post.md\ndescription: Authentication schemes for Axuall API\nschemes:\n- type: oauth2\n  name: Auth0\n  evidence: The Axuall API uses Auth0 to authenticate all API clients.\n  flows:\n  - client_credentials\n  token_url: https://api.axuall.net/v2/auth\n  how_to_obtain: Send a POST request to the token URL with client_id and client_secret in the JSON body.\ndocs: https://axuall.readme.io/reference/authenticate_user_v2_auth_post\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/authentication/axuall-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Healthcare
- Data
- Credentialing
- AI
---
