---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nudgen-net-ai-api-openapi.yml
  format: yaml
  label: Nudgen AI API
  slug: nudgen-net-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nudgen-net/openapi/nudgen-net-ai-api-openapi.yml
- filename: nudgen-net-brand-settings-api-openapi.yml
  format: yaml
  label: Nudgen Brand settings API
  slug: nudgen-net-brand-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nudgen-net/openapi/nudgen-net-brand-settings-api-openapi.yml
- filename: nudgen-net-campaigns-api-openapi.yml
  format: yaml
  label: Nudgen Campaigns API
  slug: nudgen-net-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nudgen-net/openapi/nudgen-net-campaigns-api-openapi.yml
- filename: nudgen-net-contacts-api-openapi.yml
  format: yaml
  label: Nudgen Contacts API
  slug: nudgen-net-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nudgen-net/openapi/nudgen-net-contacts-api-openapi.yml
- filename: nudgen-net-identity-api-openapi.yml
  format: yaml
  label: Nudgen Identity API
  slug: nudgen-net-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nudgen-net/openapi/nudgen-net-identity-api-openapi.yml
- filename: nudgen-net-map-leads-api-openapi.yml
  format: yaml
  label: Nudgen Map Leads API
  slug: nudgen-net-map-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nudgen-net/openapi/nudgen-net-map-leads-api-openapi.yml
- filename: nudgen-net-sending-domains-api-openapi.yml
  format: yaml
  label: Nudgen Sending domains API
  slug: nudgen-net-sending-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nudgen-net/openapi/nudgen-net-sending-domains-api-openapi.yml
- filename: nudgen-net-team-api-keys-api-openapi.yml
  format: yaml
  label: Nudgen Team API keys API
  slug: nudgen-net-team-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nudgen-net/openapi/nudgen-net-team-api-keys-api-openapi.yml
auth_types: []
description: Authentication schemes for Nudgen API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Nudgen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nudgen declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Nudgen
provider_slug: nudgen-net
scheme_count: 1
schemes:
- evidence: Personal Access Token created from Settings -> API Keys.
  header: Authorization
  how_to_obtain: Create a Personal Access Token in Settings → API Keys.
  location: header
  name: bearerAuth
  type: http-bearer
slug: nudgen-net-authentication
source_filename: nudgen-net-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.nudgen.net/api-reference/team-api-keys/list-team-api-keys.md
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.nudgen.net/api-reference/team-api-keys/list-team-api-keys.md\nsources:\n- https://docs.nudgen.net/api-reference/team-api-keys/list-team-api-keys.md\n- https://docs.nudgen.net/api-reference/team-api-keys/create-team-api-key.md\n- https://docs.nudgen.net/api-reference/team-api-keys/rotate-team-api-key.md\n- https://docs.nudgen.net/api-reference/team-api-keys/revoke-team-api-key.md\ndescription: Authentication schemes for Nudgen API\nschemes:\n- type: http-bearer\n  name: bearerAuth\n  evidence: Personal Access Token created from Settings -> API Keys.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a Personal Access Token in Settings → API Keys.\nnote: No other authentication methods (apiKey, oauth2, etc.) are documented on the provided pages.\ndocs: https://docs.nudgen.net/api-reference/team-api-keys/list-team-api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/nudgen-net/authentication/nudgen-net-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Payments
- Identity
- Communications
---
