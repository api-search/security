---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Bilg API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bilgai Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bilg declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Bilg
provider_slug: bilgai-com
scheme_count: 1
schemes:
- evidence: 'Auth: HTTP header `Authorization: Bearer blg_YOUR_KEY`'
  header: Authorization
  how_to_obtain: Create an API key in Settings → API keys → Create and bind it to a default project.
  location: header
  name: Bearer token
  type: http-bearer
slug: bilgai-com-authentication
source_filename: bilgai-com-authentication.yml
source_heading: Authentication Profile
source_url: https://app.bilgai.com/docs/connect
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://app.bilgai.com/docs/connect\nsources:\n- https://app.bilgai.com/docs/connect\ndescription: Authentication schemes for Bilg API\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Auth: HTTP header `Authorization: Bearer blg_YOUR_KEY`'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in Settings → API keys → Create and bind it to a default project.\ndocs: https://app.bilgai.com/docs/connect\n"
source_yaml_url: https://artifacts.apis.io/bilgai-com/authentication/bilgai-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Collaboration
- Knowledge Base
- Productivity
- Team Workspace
---
