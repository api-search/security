---
anonymous_access: false
api_key_in: []
api_specs:
- filename: filetourl-org-openapi-generated.yml
  format: yaml
  label: FileToUrl.org API
  slug: filetourl-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filetourl-org/openapi/_ae-authored/filetourl-org-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: FileToUrl.org Authentication
name_suffix: Authentication
oauth_flows: []
overview: FileToUrl.org declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FileToUrl.org
provider_slug: filetourl-org
scheme_count: 1
schemes:
- description: Every request needs an Authorization header with a Bearer token. Keys are generated from the account page and are prefixed `ftu_live_`.
  format: Bearer ftu_live_...
  header: Authorization
  location: header
  name: Bearer API key
  scheme: bearer
  type: http
slug: filetourl-org-authentication
source_filename: filetourl-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://filetourl.org/developers\ndocs: https://filetourl.org/developers\nschemes:\n- type: http\n  scheme: bearer\n  name: Bearer API key\n  location: header\n  header: Authorization\n  format: 'Bearer ftu_live_...'\n  description: Every request needs an Authorization header with a Bearer token. Keys are generated from the account page and are prefixed `ftu_live_`.\nkey_prefixes:\n- ftu_live_\nprovisioning: Keys are issued per account from https://filetourl.org/account; the account must be on the Developer plan.\nrevocation: Documented 401 for missing/invalid/revoked API key; 403 when the key's account is no longer on the Developer plan.\nmcp_auth:\n  transport: Bearer header on the MCP endpoint\n  endpoint: https://filetourl.org/api/mcp\n  note: \"The same API key is passed as `Authorization: Bearer ftu_live_...` in MCP client config.\"\n"
source_yaml_url: https://artifacts.apis.io/filetourl-org/authentication/filetourl-org-authentication.yml
summary_line: 1 scheme
tags:
- Company
- File Sharing
- File Hosting
- File Conversion
- URL Shortening
- Developer API
- Cloud Storage
- Document Sharing
---
