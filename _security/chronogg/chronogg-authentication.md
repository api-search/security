---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chronogg-openapi-generated.yml
  format: yaml
  label: Chronogg API
  slug: chronogg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chronogg/refs/heads/main/openapi/_ae-authored/chronogg-openapi-generated.yml
auth_types: []
description: Authentication schemes for Nexus API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Chronogg Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chronogg declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Chronogg
provider_slug: chronogg
scheme_count: 1
schemes:
- evidence: The Nexus API authenticates every request with a publisher API key , sent in the X-SHARED-SECRET request header.
  header: X-SHARED-SECRET
  how_to_obtain: Minted in the Nexus Dashboard by a publisher admin.
  location: header
  name: publisher API key
  type: apiKey
slug: chronogg-authentication
source_filename: chronogg-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.nexus.gg/authentication/api-keys
source_yaml: "generated: '2026-10-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.nexus.gg/authentication/api-keys\nsources:\n- https://docs.nexus.gg/authentication/api-keys\n- https://docs.nexus.gg/authentication/api-keys.md\n- https://docs.nexus.gg/api/operations/generateauthcode\n- https://docs.nexus.gg/api-quick-start-guide\ndescription: Authentication schemes for Nexus API\nschemes:\n- type: apiKey\n  name: publisher API key\n  evidence: The Nexus API authenticates every request with a publisher API key , sent in the X-SHARED-SECRET request header.\n  location: header\n  header: X-SHARED-SECRET\n  how_to_obtain: Minted in the Nexus Dashboard by a publisher admin.\nnote: No OAuth2 or other authentication schemes are documented on the provided pages.\ndocs: https://docs.nexus.gg/authentication/api-keys\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chronogg/refs/heads/main/authentication/chronogg-authentication.yml
summary_line: 1 scheme
tags:
- Company
---
