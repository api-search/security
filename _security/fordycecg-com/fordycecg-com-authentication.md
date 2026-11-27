---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for connecting MCP clients
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Fordyce CG Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fordyce CG declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Fordyce CG
provider_slug: fordycecg-com
scheme_count: 2
schemes:
- evidence: Any MCP client that supports sign-in (OAuth) connects with one URL and a browser sign-in
  name: OAuth
  type: oauth2
- evidence: A client without it connects with a key and one config block
  name: API Key
  type: apiKey
slug: fordycecg-com-authentication
source_filename: fordycecg-com-authentication.yml
source_heading: Authentication Profile
source_url: https://fordycecg.com/guides
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://fordycecg.com/guides\nsources:\n- https://fordycecg.com/guides\ndescription: Authentication methods for connecting MCP clients\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: Any MCP client that supports sign-in (OAuth) connects with one URL and a browser sign-in\n- type: apiKey\n  name: API Key\n  evidence: A client without it connects with a key and one config block\ndocs: https://fordycecg.com/guides\n"
source_yaml_url: https://artifacts.apis.io/fordycecg-com/authentication/fordycecg-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Software
- Small Business
- Lacrosse
- Collectibles
---
