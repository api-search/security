---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getlinkbunny-openapi-generated.yml
  format: yaml
  label: LinkBunny API
  slug: getlinkbunny-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getlinkbunny/openapi/_ae-authored/getlinkbunny-openapi-generated.yml
auth_types: []
description: LinkBunny authenticates API requests using a bearer token supplied in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: LinkBunny Authentication
name_suffix: Authentication
oauth_flows: []
overview: LinkBunny declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: LinkBunny
provider_slug: getlinkbunny
scheme_count: 1
schemes:
- evidence: 'printf ''header = "Authorization: Bearer %s"\n'' "$LINKBUNNY_API_TOKEN"'
  header: Authorization
  how_to_obtain: Create or rotate the token in the LinkBunny Account page and store it in a private secret store or environment variable.
  location: header
  name: LinkBunny API token
  type: http-bearer
slug: getlinkbunny-authentication
source_filename: getlinkbunny-authentication.yml
source_heading: Authentication Profile
source_url: https://getlinkbunny.com/mcp
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://getlinkbunny.com/mcp\nsources:\n- https://getlinkbunny.com/mcp\n- https://getlinkbunny.com/docs/agents\n- https://getlinkbunny.com/tools/backlink-placement-checker#claude\n- https://getlinkbunny.com/claude-code\ndescription: LinkBunny authenticates API requests using a bearer token supplied in the Authorization header.\nschemes:\n- type: http-bearer\n  name: LinkBunny API token\n  evidence: 'printf ''header = \"Authorization: Bearer %s\"\\n'' \"$LINKBUNNY_API_TOKEN\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create or rotate the token in the LinkBunny Account page and store it in a private secret store or environment variable.\nnote: No OAuth2, apiKey, or other authentication methods are documented on the provided pages.\ndocs: https://getlinkbunny.com/mcp\n"
source_yaml_url: https://artifacts.apis.io/getlinkbunny/authentication/getlinkbunny-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Backlinks
- SEO
- Marketplace
- Automation
---
