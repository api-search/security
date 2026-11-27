---
anonymous_access: false
api_key_in: []
api_specs:
- filename: letsaskit-com-openapi-generated.yml
  format: yaml
  label: LetsAskIt API
  slug: letsaskit-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/letsaskit-com/openapi/_ae-authored/letsaskit-com-openapi-generated.yml
auth_types: []
description: Authentication schemes for LetsAskIt as documented.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: LetsAskIt Authentication
name_suffix: Authentication
oauth_flows: []
overview: LetsAskIt declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: LetsAskIt
provider_slug: letsaskit-com
scheme_count: 1
schemes:
- evidence: 'Auth: Authorization: Bearer <team-api-key>'
  header: Authorization
  how_to_obtain: Email [email protected] from the address that will own the subscription; the reply carries your key.
  location: header
  name: Team API key
  type: http-bearer
slug: letsaskit-com-authentication
source_filename: letsaskit-com-authentication.yml
source_heading: Authentication Profile
source_url: https://letsaskit.com/docs/getting-started
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://letsaskit.com/docs/getting-started\nsources:\n- https://letsaskit.com/docs/getting-started\n- https://letsaskit.com/docs/mcp-setup\ndescription: Authentication schemes for LetsAskIt as documented.\nschemes:\n- type: http-bearer\n  name: Team API key\n  evidence: 'Auth: Authorization: Bearer <team-api-key>'\n  location: header\n  header: Authorization\n  how_to_obtain: Email [email protected] from the address that will own the subscription; the reply carries your key.\ndocs: https://letsaskit.com/docs/getting-started\n"
source_yaml_url: https://artifacts.apis.io/letsaskit-com/authentication/letsaskit-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Content Creation
- Marketing
- Automation
---
