---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes documented for SKYVVA
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Skyvva Authentication
name_suffix: Authentication
oauth_flows: []
overview: SKYVVA declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: SKYVVA
provider_slug: skyvva
scheme_count: 2
schemes:
- evidence: 'Basic Authentication: This authentication method involves sending credentials (usually a username and password) with each request made from the agent to Salesforce.'
  name: Basic
  type: http-basic
- evidence: 'URL: https://enterprise-ruby-3909-dev-ed.scratch.my.salesforce.com/services/oauth2/token'
  flows:
  - client_credentials
  how_to_obtain: Obtain the client ID and client secret from the connected app’s Consumer Key and Consumer Secret.
  name: OAuth2 Client-Credential
  token_url: https://enterprise-ruby-3909-dev-ed.scratch.my.salesforce.com/services/oauth2/token
  type: oauth2
slug: skyvva-authentication
source_filename: skyvva-authentication.yml
source_heading: Authentication Profile
source_url: https://help.skyvva.com/articles/156-1-api-key-authentication.html
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.skyvva.com/articles/156-1-api-key-authentication.html\nsources:\n- https://help.skyvva.com/articles/156-1-api-key-authentication.html\n- https://help.skyvva.com/articles/156-2-salesforce-authentication-provider-aws-signature.html\n- https://help.skyvva.com/articles/how-to-generate-an-access-token-using-oauth-2-0-client-credentials-flow-with-skyvva-permissions.html\n- https://help.skyvva.com/articles/11-how-to-use-oauth-grant-type-on-agent-control-board.html\ndescription: Authentication schemes documented for SKYVVA\nschemes:\n- type: http-basic\n  name: Basic\n  evidence: 'Basic Authentication: This authentication method involves sending credentials (usually a username and password) with each request\n    made from the agent to Salesforce.'\n- type: oauth2\n  name: OAuth2 Client-Credential\n  evidence: 'URL: https://enterprise-ruby-3909-dev-ed.scratch.my.salesforce.com/services/oauth2/token'\n\
  \  flows:\n  - client_credentials\n  token_url: https://enterprise-ruby-3909-dev-ed.scratch.my.salesforce.com/services/oauth2/token\n  how_to_obtain: Obtain the client ID and client secret from the connected app’s Consumer Key and Consumer Secret.\ndocs: https://help.skyvva.com/articles/156-1-api-key-authentication.html\n"
source_yaml_url: https://artifacts.apis.io/skyvva/authentication/skyvva-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Integration
- Salesforce
- ERP
- Middleware-free
---
