---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for DocDriven Code Assistant via GitHub
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Docdriven Authentication
name_suffix: Authentication
oauth_flows: []
overview: DocDriven declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DocDriven
provider_slug: docdriven
scheme_count: 1
schemes:
- evidence: To use the DocDriven Code Assistant, you need to authenticate with your GitHub account.
  flows:
  - authorization_code
  how_to_obtain: Redirect to GitHub login and authorize DocDriven.
  name: GitHub
  type: oauth2
slug: docdriven-authentication
source_filename: docdriven-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.docdriven.com/docs/code-assistant/github
source_yaml: "generated: '2026-10-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.docdriven.com/docs/code-assistant/github\nsources:\n- https://docs.docdriven.com/docs/code-assistant/github\ndescription: Authentication for DocDriven Code Assistant via GitHub\nschemes:\n- type: oauth2\n  name: GitHub\n  evidence: To use the DocDriven Code Assistant, you need to authenticate with your GitHub account.\n  flows:\n  - authorization_code\n  how_to_obtain: Redirect to GitHub login and authorize DocDriven.\ndocs: https://docs.docdriven.com/docs/code-assistant/github\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docdriven/refs/heads/main/authentication/docdriven-authentication.yml
summary_line: 1 scheme
tags:
- Company
- API Design
- Artificial Intelligence
- Collaboration
- Documentation
- Platform
---
