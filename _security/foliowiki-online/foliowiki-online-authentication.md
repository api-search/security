---
anonymous_access: false
api_key_in: []
api_specs:
- filename: foliowiki-online-openapi-generated.yml
  format: yaml
  label: Folio API
  slug: foliowiki-online-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foliowiki-online/openapi/_ae-authored/foliowiki-online-openapi-generated.yml
auth_types: []
description: 'Folio supports two authentication methods for MCP: a personal access token used as a bearer token in the Authorization header, and OAuth 2.0 with PKCE using the authorization code flow.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Folio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Folio declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Folio
provider_slug: foliowiki-online
scheme_count: 2
schemes:
- evidence: Personal access token. You create it under the user menu, API tokens. It starts with folio_pat_ , is shown once and has the scope read or write.
  header: Authorization
  how_to_obtain: Create a token under the user menu → API tokens; the token is shown once.
  location: header
  name: Personal Access Token
  scopes:
  - read
  - write
  type: apiKey
- evidence: OAuth access token. Used by claude.ai, Claude Desktop and ChatGPT. It starts with folio_oat_ and lasts one hour.
  flows:
  - authorizationCode
  how_to_obtain: Sign in to Folio via the OAuth consent screen; the client uses PKCE and the authorization code flow.
  name: OAuth 2.0
  scopes:
  - read
  - write
  type: oauth2
slug: foliowiki-online-authentication
source_filename: foliowiki-online-authentication.yml
source_heading: Authentication Profile
source_url: https://foliowiki.online/blog/mcp-security-wiki-oauth-tokens-permissions/
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://foliowiki.online/blog/mcp-security-wiki-oauth-tokens-permissions/\nsources:\n- https://foliowiki.online/blog/mcp-security-wiki-oauth-tokens-permissions/\n- https://foliowiki.online/integrations/claude/#faq\n- https://foliowiki.online/integrations/cursor/#faq\n- https://foliowiki.online/integrations/codex/#faq\ndescription: 'Folio supports two authentication methods for MCP: a personal access token used as a bearer token in the Authorization header, and\n  OAuth 2.0 with PKCE using the authorization code flow.'\nschemes:\n- type: apiKey\n  name: Personal Access Token\n  evidence: Personal access token. You create it under the user menu, API tokens. It starts with folio_pat_ , is shown once and has the scope\n    read or write.\n  location: header\n  header: Authorization\n  scopes:\n  - read\n  - write\n  how_to_obtain: Create a token under the user menu → API tokens; the\
  \ token is shown once.\n- type: oauth2\n  name: OAuth 2.0\n  evidence: OAuth access token. Used by claude.ai, Claude Desktop and ChatGPT. It starts with folio_oat_ and lasts one hour.\n  flows:\n  - authorizationCode\n  scopes:\n  - read\n  - write\n  how_to_obtain: Sign in to Folio via the OAuth consent screen; the client uses PKCE and the authorization code flow.\ndocs: https://foliowiki.online/blog/mcp-security-wiki-oauth-tokens-permissions/\n"
source_yaml_url: https://artifacts.apis.io/foliowiki-online/authentication/foliowiki-online-authentication.yml
summary_line: 2 schemes
tags:
- Wiki
- Documentation
- Open Source
- Self-Hosted
- Git-based
- Collaboration
- AI Assistant
- Docs as Code
---
