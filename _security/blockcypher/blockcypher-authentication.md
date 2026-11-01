---
anonymous_access: false
api_key_in: []
auth_types: []
description: BlockCypher uses an API token passed as a query parameter.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Blockcypher Authentication
name_suffix: Authentication
oauth_flows: []
overview: BlockCypher declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: BlockCypher
provider_slug: blockcypher
scheme_count: 1
schemes:
- evidence: curl http://api.blockcypher.com/v1/btc/main?token=$TOKEN
  how_to_obtain: Create an account on the developer portal and copy‑paste the token.
  location: query
  name: token
  type: apiKey
slug: blockcypher-authentication
source_filename: blockcypher-authentication.yml
source_heading: Authentication Profile
source_url: https://www.blockcypher.com/getting-started.html
source_yaml: "generated: '2026-10-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.blockcypher.com/getting-started.html\nsources:\n- https://www.blockcypher.com/getting-started.html\ndescription: BlockCypher uses an API token passed as a query parameter.\nschemes:\n- type: apiKey\n  name: token\n  evidence: curl http://api.blockcypher.com/v1/btc/main?token=$TOKEN\n  location: query\n  how_to_obtain: Create an account on the developer portal and copy‑paste the token.\ndocs: https://www.blockcypher.com/getting-started.html\n"
source_yaml_url: https://artifacts.apis.io/blockcypher/authentication/blockcypher-authentication.yml
summary_line: 1 scheme
tags:
- APIs
- Blockchain
- Infrastructure
- Enterprise
---
