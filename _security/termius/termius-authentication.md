---
api_key_in: []
api_specs:
- filename: termius-api-bridge-openapi-original.yml
  format: yaml
  label: Termius API Bridge
  slug: termius-api-bridge
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/termius/refs/heads/main/openapi/termius-api-bridge-openapi-original.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Termius Authentication
name_suffix: Authentication
oauth_flows: []
overview: Termius declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Termius
provider_slug: termius
scheme_count: 0
schemes: []
slug: termius-authentication
source_filename: termius-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://termius.com/api-docs/, https://termius.com/blog/keep-connection-details-up-to-date-with-api-bridge\ndocs: https://support.termius.com/hc/en-us/\nsummary:\n  types: []            # no securitySchemes declared in the OpenAPI\n  model: api-bridge-key\ndetail: >-\n  The Termius API Bridge OpenAPI declares no HTTP-layer securitySchemes: the REST\n  API is served by a container the customer runs locally (default localhost:8080)\n  and is reached over the local network. Trust is established out of band — using\n  the API Bridge requires a Termius Team plan, and an API Bridge is provisioned\n  from the Team's API Bridge page, which issues the key the bridge uses to\n  authenticate to the Termius cloud and to encrypt infrastructure data locally\n  before pushing it into the Team vault. There is no public OAuth or API-key\n  scheme for direct cloud API access.\nschemes: []\nplan_requirement: Team\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/termius/refs/heads/main/authentication/termius-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Enterprise Saas
- SSH
- SSH Client
- Terminal
- Developer Tools
- DevOps
- Infrastructure
- Security
- Remote Access
---
