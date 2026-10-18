---
anonymous_access: false
api_key_in: []
api_specs:
- filename: contraforce-agent-tools-api-openapi.yml
  format: yaml
  label: Contraforce Agent Tools API
  slug: contraforce-agent-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-agent-tools-api-openapi.yml
- filename: contraforce-azure-resources-api-openapi.yml
  format: yaml
  label: Contraforce Azure resources API
  slug: contraforce-azure-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-azure-resources-api-openapi.yml
- filename: contraforce-cross-workspace-data-sources-api-openapi.yml
  format: yaml
  label: Contraforce Cross-workspace data sources API
  slug: contraforce-cross-workspace-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-cross-workspace-data-sources-api-openapi.yml
- filename: contraforce-cross-workspace-gamebooks-api-openapi.yml
  format: yaml
  label: Contraforce Cross-workspace gamebooks API
  slug: contraforce-cross-workspace-gamebooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-cross-workspace-gamebooks-api-openapi.yml
- filename: contraforce-cross-workspace-incidents-api-openapi.yml
  format: yaml
  label: Contraforce Cross-workspace incidents API
  slug: contraforce-cross-workspace-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-cross-workspace-incidents-api-openapi.yml
- filename: contraforce-data-sources-api-openapi.yml
  format: yaml
  label: Contraforce Data sources API
  slug: contraforce-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-data-sources-api-openapi.yml
- filename: contraforce-export-api-openapi.yml
  format: yaml
  label: Contraforce Export API
  slug: contraforce-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-export-api-openapi.yml
- filename: contraforce-gamebooks-api-openapi.yml
  format: yaml
  label: Contraforce Gamebooks API
  slug: contraforce-gamebooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-gamebooks-api-openapi.yml
- filename: contraforce-incidents-api-openapi.yml
  format: yaml
  label: Contraforce Incidents API
  slug: contraforce-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-incidents-api-openapi.yml
- filename: contraforce-investigation-api-openapi.yml
  format: yaml
  label: Contraforce Investigation API
  slug: contraforce-investigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-investigation-api-openapi.yml
- filename: contraforce-service-accounts-api-openapi.yml
  format: yaml
  label: Contraforce Service accounts API
  slug: contraforce-service-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-service-accounts-api-openapi.yml
- filename: contraforce-service-tickets-api-openapi.yml
  format: yaml
  label: Contraforce Service tickets API
  slug: contraforce-service-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-service-tickets-api-openapi.yml
- filename: contraforce-users-api-openapi.yml
  format: yaml
  label: Contraforce Users API
  slug: contraforce-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-users-api-openapi.yml
- filename: contraforce-webhooks-api-openapi.yml
  format: yaml
  label: Contraforce Webhooks API
  slug: contraforce-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-webhooks-api-openapi.yml
auth_types: []
description: Authentication methods for ContraForce API as documented.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Contraforce Authentication
name_suffix: Authentication
oauth_flows: []
overview: Contraforce declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Contraforce
provider_slug: contraforce
scheme_count: 1
schemes:
- evidence: Service accounts use **HTTP Basic authentication** (RFC 7617). Encode `ClientId:ClientSecret` in Base64 and send it in the `Authorization` header.
  header: Authorization
  how_to_obtain: Create a service account in the ContraForce portal to receive a Client ID and Client Secret.
  location: header
  name: HTTP Basic
  type: http-basic
slug: contraforce-authentication
source_filename: contraforce-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.contraforce.com/guides/general-support/service-accounts.md
source_yaml: "generated: '2026-10-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.contraforce.com/guides/general-support/service-accounts.md\nsources:\n- https://docs.contraforce.com/guides/general-support/service-accounts.md\n- https://docs.contraforce.com/api-reference/webhooks/update-webhook-credentials.md\n- https://docs.contraforce.com/guides/getting-started/command-dashboard.md\n- https://docs.contraforce.com/guides/getting-started/quick-actions.md\ndescription: Authentication methods for ContraForce API as documented.\nschemes:\n- type: http-basic\n  name: HTTP Basic\n  evidence: Service accounts use **HTTP Basic authentication** (RFC 7617). Encode `ClientId:ClientSecret` in Base64 and send it in the `Authorization`\n    header.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a service account in the ContraForce portal to receive a Client ID and Client Secret.\ndocs: https://docs.contraforce.com/guides/general-support/service-accounts.md\n\
  note: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/authentication/contraforce-authentication.yml
summary_line: 1 scheme
tags:
- Security
- Software-as-a-Service
- Cybersecurity
- Microsoft
- MSP
---
