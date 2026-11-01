---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mimecast-com-openapi-generated.yml
  format: yaml
  label: ProjectDiscovery API
  slug: mimecast-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mimecast-com/openapi/_ae-authored/mimecast-com-openapi-generated.yml
auth_types: []
description: Authentication methods for Neo API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mimecast Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: ProjectDiscovery declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ProjectDiscovery
provider_slug: mimecast-com
scheme_count: 1
schemes:
- evidence: 'Pass the key in the `X-Api-Key` header on every request:'
  header: X-Api-Key
  location: header
  name: X-Api-Key
  type: apiKey
slug: mimecast-com-authentication
source_filename: mimecast-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.neo.projectdiscovery.io/platform/settings/api-key.md
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.neo.projectdiscovery.io/platform/settings/api-key.md\nsources:\n- https://docs.neo.projectdiscovery.io/platform/settings/api-key.md\n- https://docs.neo.projectdiscovery.io/api-reference/github/github-oauth-callback.md\n- https://docs.neo.projectdiscovery.io/api-reference/github/initiate-github-oauth.md\n- https://docs.neo.projectdiscovery.io/api-reference/slack/slack-oauth-callback.md\ndescription: Authentication methods for Neo API\nschemes:\n- type: apiKey\n  name: X-Api-Key\n  evidence: 'Pass the key in the `X-Api-Key` header on every request:'\n  location: header\n  header: X-Api-Key\ndocs: https://docs.neo.projectdiscovery.io/platform/settings/api-key.md\n"
source_yaml_url: https://artifacts.apis.io/mimecast-com/authentication/mimecast-com-authentication.yml
summary_line: 1 scheme
tags:
- Vulnerability Management
- Offensive Security
- Cloud Security
- Open Source Tools
---
