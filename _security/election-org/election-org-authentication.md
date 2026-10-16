---
anonymous_access: false
api_key_in: []
api_specs:
- filename: election-org-openapi-openapi.json
  format: json
  label: Election.org Public Data API Openapi API
  slug: election-org-public-data-api-openapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/election-org/refs/heads/main/openapi/_original/election-org-openapi-openapi.json
auth_types: []
description: Authentication for Election.org Public Data API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Election Org Authentication
name_suffix: Authentication
oauth_flows: []
overview: Election.org Public Data API declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Election.org Public Data API
provider_slug: election-org
scheme_count: 1
schemes:
- evidence: 'fetch("https://election.org/api/developers/data/committees?q=buckeye", { headers: { Authorization: "Bearer " + process.env.ELECTION_API_KEY }})'
  header: Authorization
  how_to_obtain: Free API key via registration form
  location: header
  name: Bearer
  type: http-bearer
slug: election-org-authentication
source_filename: election-org-authentication.yml
source_heading: Authentication Profile
source_url: https://election.org/data/api/access
source_yaml: "generated: '2026-10-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://election.org/data/api/access\nsources:\n- https://election.org/data/api/access\ndescription: Authentication for Election.org Public Data API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'fetch(\"https://election.org/api/developers/data/committees?q=buckeye\", { headers: { Authorization: \"Bearer \" + process.env.ELECTION_API_KEY\n    }})'\n  location: header\n  header: Authorization\n  how_to_obtain: Free API key via registration form\ndocs: https://election.org/data/api/access\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/election-org/refs/heads/main/authentication/election-org-authentication.yml
summary_line: 1 scheme
tags:
- Elections
- Public Records
- Data API
- Campaign Finance
- Government
- Political Data
---
