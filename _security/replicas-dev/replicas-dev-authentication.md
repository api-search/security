---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Replicas API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Replicas Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Replicas declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Replicas
provider_slug: replicas-dev
scheme_count: 1
schemes:
- evidence: Organization or personal API key from **Settings → API Keys**.
  header: Authorization
  how_to_obtain: Organization or personal API key from Settings → API Keys.
  location: header
  name: apiKey
  type: http-bearer
slug: replicas-dev-authentication
source_filename: replicas-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.replicas.dev/api-reference/plugins/start-plugin-oauth.md
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.replicas.dev/api-reference/plugins/start-plugin-oauth.md\nsources:\n- https://docs.replicas.dev/api-reference/plugins/start-plugin-oauth.md\n- https://docs.replicas.dev/admin/credentials.md\n- https://docs.replicas.dev/api-reference/agent-credentials/list-models.md\n- https://docs.replicas.dev/api-reference/agent-credentials/get-organization-credential.md\ndescription: Authentication schemes for Replicas API\nschemes:\n- type: http-bearer\n  name: apiKey\n  evidence: Organization or personal API key from **Settings → API Keys**.\n  location: header\n  header: Authorization\n  how_to_obtain: Organization or personal API key from Settings → API Keys.\ndocs: https://docs.replicas.dev/api-reference/plugins/start-plugin-oauth.md\n"
source_yaml_url: https://artifacts.apis.io/replicas-dev/authentication/replicas-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Cloud
- Platform
- Development
---
