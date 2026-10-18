---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for localscreenshot
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Localscreenshot Authentication
name_suffix: Authentication
oauth_flows: []
overview: localscreenshot declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: localscreenshot
provider_slug: localscreenshot
scheme_count: 1
schemes:
- evidence: Put it in the Authorization header, after the word Bearer .
  header: Authorization
  how_to_obtain: Create and copy a key in the dashboard under Connect.
  location: header
  name: Bearer token
  type: http-bearer
slug: localscreenshot-authentication
source_filename: localscreenshot-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.localscreenshot.com/auth
source_yaml: "generated: '2026-10-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.localscreenshot.com/auth\nsources:\n- https://docs.localscreenshot.com/auth\n- https://docs.langchain.com/oss/python/langchain/mcp/auth\n- https://antigravity.google/docs/cli/install\n- https://support.claude.com/en/articles/11175166-get-started-with-custom-connectors-using-remote-mcp\ndescription: Authentication schemes for localscreenshot\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: Put it in the Authorization header, after the word Bearer .\n  location: header\n  header: Authorization\n  how_to_obtain: Create and copy a key in the dashboard under Connect.\ndocs: https://docs.localscreenshot.com/auth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/localscreenshot/refs/heads/main/authentication/localscreenshot-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Screenshots
- Artificial Intelligence
- Automation
---
