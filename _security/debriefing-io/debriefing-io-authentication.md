---
anonymous_access: false
api_key_in: []
api_specs:
- filename: debriefing-io-openapi.json
  format: json
  label: Debriefing Read API
  slug: debriefing-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debriefing-io/openapi/debriefing-io-openapi.json
- filename: debriefing-io-battlecards-api-openapi.yml
  format: yaml
  label: Debriefing Battlecards API
  slug: debriefing-io-battlecards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debriefing-io/openapi/debriefing-io-battlecards-api-openapi.yml
- filename: debriefing-io-competitors-api-openapi.yml
  format: yaml
  label: Debriefing Competitors API
  slug: debriefing-io-competitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debriefing-io/openapi/debriefing-io-competitors-api-openapi.yml
- filename: debriefing-io-digests-api-openapi.yml
  format: yaml
  label: Debriefing Digests API
  slug: debriefing-io-digests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debriefing-io/openapi/debriefing-io-digests-api-openapi.yml
- filename: debriefing-io-signals-api-openapi.yml
  format: yaml
  label: Debriefing Signals API
  slug: debriefing-io-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debriefing-io/openapi/debriefing-io-signals-api-openapi.yml
auth_types: []
description: Authentication methods for Debriefing as documented on the provider pages.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Debriefing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Debriefing declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Debriefing
provider_slug: debriefing-io
scheme_count: 1
schemes:
- authorize_url: https://debriefing.io/oauth/authorize
  evidence: Authorization code flow with PKCE (`S256` only) at https://debriefing.io/oauth/authorize. The person signs in and approves on a consent screen.
  flows:
  - authorization_code
  how_to_obtain: Client registration via dynamic registration (POST https://debriefing.io/oauth/register) or by providing a client_id metadata document URL. The person then authorizes the client through the consent screen.
  name: OAuth 2.1 Authorization Code with PKCE
  scopes:
  - read
  - write
  - spend
  - offline_access
  type: oauth2
slug: debriefing-io-authentication
source_filename: debriefing-io-authentication.yml
source_heading: Authentication Profile
source_url: https://debriefing.io/.well-known/oauth-protected-resource/mcp
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://debriefing.io/.well-known/oauth-protected-resource/mcp\nsources:\n- https://debriefing.io/.well-known/oauth-protected-resource/mcp\n- https://debriefing.io/.well-known/oauth-authorization-server\n- https://debriefing.io/intel/klue-icarus-oauth-salesforce-supply-chain-breach.md\n- https://debriefing.io/auth.md\ndescription: Authentication methods for Debriefing as documented on the provider pages.\nschemes:\n- type: oauth2\n  name: OAuth 2.1 Authorization Code with PKCE\n  evidence: Authorization code flow with PKCE (`S256` only) at https://debriefing.io/oauth/authorize. The person signs in and approves on a consent\n    screen.\n  flows:\n  - authorization_code\n  authorize_url: https://debriefing.io/oauth/authorize\n  scopes:\n  - read\n  - write\n  - spend\n  - offline_access\n  how_to_obtain: Client registration via dynamic registration (POST https://debriefing.io/oauth/register)\
  \ or by providing a client_id metadata\n    document URL. The person then authorizes the client through the consent screen.\ndocs: https://debriefing.io/.well-known/oauth-protected-resource/mcp\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/debriefing-io/authentication/debriefing-io-authentication.yml
summary_line: 1 scheme
tags:
- Competitive Intelligence
- Software-as-a-Service
- B2B
- Monitoring
- Small Business
---
