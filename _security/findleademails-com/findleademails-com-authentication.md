---
anonymous_access: false
api_key_in: []
auth_types: []
description: FindLeadEmails supports authentication via OAuth sign‑in or by providing an API key as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: FindLeadEmails Authentication
name_suffix: Authentication
oauth_flows: []
overview: FindLeadEmails declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FindLeadEmails
provider_slug: findleademails-com
scheme_count: 1
schemes:
- evidence: paste the key from the Developers page into the Authorization header as Bearer YOUR_API_KEY.
  header: Authorization
  how_to_obtain: Create a key on the Developers page, copy it when shown, and use it as the Bearer token in the Authorization header.
  location: header
  name: API key
  type: http-bearer
slug: findleademails-com-authentication
source_filename: findleademails-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.findleademails.com/docs/mcp
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.findleademails.com/docs/mcp\nsources:\n- https://www.findleademails.com/docs/mcp\n- https://www.findleademails.com/dns\ndescription: FindLeadEmails supports authentication via OAuth sign‑in or by providing an API key as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: paste the key from the Developers page into the Authorization header as Bearer YOUR_API_KEY.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key on the Developers page, copy it when shown, and use it as the Bearer token in the Authorization header.\ndocs: https://www.findleademails.com/docs/mcp\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/findleademails-com/authentication/findleademails-com-authentication.yml
summary_line: 1 scheme
tags:
- Email Finder
- Email Verification
- Bulk Processing
---
