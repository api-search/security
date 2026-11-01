---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pastesheet-com-openapi-generated.yml
  format: yaml
  label: pastesheet-com API
  slug: pastesheet-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pastesheet-com/openapi/_ae-authored/pastesheet-com-openapi-generated.yml
auth_types: []
description: Authentication methods for Google Sheets API as described by PasteSheet.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Pastesheet Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: pastesheet-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: pastesheet-com
provider_slug: pastesheet-com
scheme_count: 2
schemes:
- evidence: For a public spreadsheet, the key travels as the `key` query parameter.
  how_to_obtain: Create an API key in Google Cloud Console and include it as the `key` query parameter.
  location: query
  name: API key
  type: apiKey
- evidence: 'The access token belongs in an `Authorization: Bearer` header.'
  header: Authorization
  how_to_obtain: Obtain an OAuth client, have the user consent, and exchange the authorization code for an access token.
  location: header
  name: OAuth 2.0
  type: http-bearer
slug: pastesheet-com-authentication
source_filename: pastesheet-com-authentication.yml
source_heading: Authentication Profile
source_url: https://pastesheet.com/guides/google-sheets-api-authentication.md
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://pastesheet.com/guides/google-sheets-api-authentication.md\nsources:\n- https://pastesheet.com/guides/google-sheets-api-authentication.md\n- https://pastesheet.com/guides/google-sheets-api-without-api-key.md\ndescription: Authentication methods for Google Sheets API as described by PasteSheet.\nschemes:\n- type: apiKey\n  name: API key\n  evidence: For a public spreadsheet, the key travels as the `key` query parameter.\n  location: query\n  how_to_obtain: Create an API key in Google Cloud Console and include it as the `key` query parameter.\n- type: http-bearer\n  name: OAuth 2.0\n  evidence: 'The access token belongs in an `Authorization: Bearer` header.'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain an OAuth client, have the user consent, and exchange the authorization code for an access token.\nnote: OAuth flow URLs and scopes are not explicitly\
  \ listed on the pages, so they are omitted. 1 extracted row(s) were dropped because their quote\n  was not on the page.\ndocs: https://pastesheet.com/guides/google-sheets-api-authentication.md\n"
source_yaml_url: https://artifacts.apis.io/pastesheet-com/authentication/pastesheet-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- API
- GoogleSheets
- NoCode
- AI
---
