---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication uses a Bearer token passed in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: TrueClicks Authentication
name_suffix: Authentication
oauth_flows: []
overview: TrueClicks declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: TrueClicks
provider_slug: trueclicks-com
scheme_count: 1
schemes:
- evidence: '"Authorization: Bearer {YOUR_GPT_TOKEN}"'
  header: Authorization
  how_to_obtain: Generate a GPT token from gaql.app as described in the standard setup.
  location: header
  name: Bearer token
  type: http-bearer
slug: trueclicks-com-authentication
source_filename: trueclicks-com-authentication.yml
source_heading: Authentication Profile
source_url: https://help.trueclicks.com/en/articles/15080110-claude-ai-how-to-connect-mcps-securely-advanced-setup.md
source_yaml: "generated: '2026-11-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.trueclicks.com/en/articles/15080110-claude-ai-how-to-connect-mcps-securely-advanced-setup.md\nsources:\n- https://help.trueclicks.com/en/articles/15080110-claude-ai-how-to-connect-mcps-securely-advanced-setup.md\ndescription: Authentication uses a Bearer token passed in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: '\"Authorization: Bearer {YOUR_GPT_TOKEN}\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a GPT token from gaql.app as described in the standard setup.\ndocs: https://help.trueclicks.com/en/articles/15080110-claude-ai-how-to-connect-mcps-securely-advanced-setup.md\n"
source_yaml_url: https://artifacts.apis.io/trueclicks-com/authentication/trueclicks-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- PPC
- Marketing
- Advertising
- SaaS
---
