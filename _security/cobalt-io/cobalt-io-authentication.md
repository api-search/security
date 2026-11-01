---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Cobalt API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cobalt Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cobalt declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Cobalt
provider_slug: cobalt-io
scheme_count: 2
schemes:
- evidence: To authenticate to the Cobalt API, you need an access token.
  header: Authorization
  how_to_obtain: Create a personal API token in the Cobalt UI (see Create a Personal Cobalt API Token page).
  location: header
  name: Personal API Token
  type: http-bearer
- evidence: Include the organization token in the X-Org-Token header of your requests.
  header: X-Org-Token
  how_to_obtain: Retrieve the organization token via the API using a personal API token (see Get an Organization Token page).
  location: header
  name: Organization Token
  type: apiKey
slug: cobalt-io-authentication
source_filename: cobalt-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.cobalt.io/articles/target-authentication-HPNawf0VBJ.md
source_yaml: "generated: '2026-10-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.cobalt.io/articles/target-authentication-HPNawf0VBJ.md\nsources:\n- https://docs.cobalt.io/articles/target-authentication-HPNawf0VBJ.md\n- https://docs.cobalt.io/articles/revoke-your-personal-cobalt-api-tokens-1QJ0vt4nzg.md\n- https://docs.cobalt.io/articles/get-an-organization-token-RlqtesM1QN.md\n- https://docs.cobalt.io/articles/create-a-personal-cobalt-api-token-LT9Nl8EAVR.md\ndescription: Authentication methods for Cobalt API\nschemes:\n- type: http-bearer\n  name: Personal API Token\n  evidence: To authenticate to the Cobalt API, you need an access token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a personal API token in the Cobalt UI (see Create a Personal Cobalt API Token page).\n- type: apiKey\n  name: Organization Token\n  evidence: Include the organization token in the X-Org-Token header of your requests.\n  location: header\n \
  \ header: X-Org-Token\n  how_to_obtain: Retrieve the organization token via the API using a personal API token (see Get an Organization Token page).\ndocs: https://docs.cobalt.io/articles/target-authentication-HPNawf0VBJ.md\n"
source_yaml_url: https://artifacts.apis.io/cobalt-io/authentication/cobalt-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Security
- PenetrationTesting
- OffensiveSecurity
- SaaS
- Platform
---
