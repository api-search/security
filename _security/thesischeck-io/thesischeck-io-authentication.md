---
anonymous_access: false
api_key_in: []
api_specs:
- filename: thesischeck-io-openapi-generated.yml
  format: yaml
  label: ThesisCheck API
  slug: thesischeck-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thesischeck-io/openapi/_ae-authored/thesischeck-io-openapi-generated.yml
auth_types: []
description: Authentication methods as described on ThesisCheck documentation pages.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: ThesisCheck Authentication
name_suffix: Authentication
oauth_flows: []
overview: ThesisCheck declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ThesisCheck
provider_slug: thesischeck-io
scheme_count: 2
schemes:
- evidence: Auth OAuth 2.1 with PKCE, with tc_ API key bearer fallback
  flows:
  - authorization_code
  how_to_obtain: Sign in to ThesisCheck in the browser and authorize MCP access as part of the OAuth connection flow.
  name: OAuth 2.1 with PKCE
  scopes:
  - mcp:tools
  type: oauth2
- evidence: Auth OAuth 2.1 with PKCE, with tc_ API key bearer fallback
  header: Authorization
  how_to_obtain: Provide a tc_ prefixed API key as a Bearer token in the Authorization header.
  name: API key bearer fallback
  type: http-bearer
slug: thesischeck-io-authentication
source_filename: thesischeck-io-authentication.yml
source_heading: Authentication Profile
source_url: https://thesischeck.io/docs/getting-started/overview
source_yaml: "generated: '2026-11-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://thesischeck.io/docs/getting-started/overview\nsources:\n- https://thesischeck.io/docs/getting-started/overview\n- https://thesischeck.io/docs/integrations/claude-mcp-setup\ndescription: Authentication methods as described on ThesisCheck documentation pages.\nschemes:\n- type: oauth2\n  name: OAuth 2.1 with PKCE\n  evidence: Auth OAuth 2.1 with PKCE, with tc_ API key bearer fallback\n  flows:\n  - authorization_code\n  scopes:\n  - mcp:tools\n  how_to_obtain: Sign in to ThesisCheck in the browser and authorize MCP access as part of the OAuth connection flow.\n- type: http-bearer\n  name: API key bearer fallback\n  evidence: Auth OAuth 2.1 with PKCE, with tc_ API key bearer fallback\n  header: Authorization\n  how_to_obtain: Provide a tc_ prefixed API key as a Bearer token in the Authorization header.\ndocs: https://thesischeck.io/docs/getting-started/overview\n"
source_yaml_url: https://artifacts.apis.io/thesischeck-io/authentication/thesischeck-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Finance
- Investment
- Research
- Data
---
