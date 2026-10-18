---
anonymous_access: false
api_key_in: []
auth_types: []
description: CompanyEnrich uses an API key that is sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Companyenrich Authentication
name_suffix: Authentication
oauth_flows: []
overview: CompanyEnrich declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CompanyEnrich
provider_slug: companyenrich
scheme_count: 1
schemes:
- evidence: Replace <YOUR TOKEN> with your CompanyEnrich API key (get one at companyenrich.com).
  header: Authorization
  how_to_obtain: CompanyEnrich API key (get one at companyenrich.com)
  location: header
  name: Bearer
  type: http-bearer
slug: companyenrich-authentication
source_filename: companyenrich-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.companyenrich.com/docs/getting-started.md
source_yaml: "generated: '2026-10-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.companyenrich.com/docs/getting-started.md\nsources:\n- https://docs.companyenrich.com/docs/getting-started.md\n- https://docs.companyenrich.com/docs/getting-started\n- https://docs.companyenrich.com/docs/mcp-server\ndescription: CompanyEnrich uses an API key that is sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Replace <YOUR TOKEN> with your CompanyEnrich API key (get one at companyenrich.com).\n  location: header\n  header: Authorization\n  how_to_obtain: CompanyEnrich API key (get one at companyenrich.com)\ndocs: https://docs.companyenrich.com/docs/getting-started.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/companyenrich/refs/heads/main/authentication/companyenrich-authentication.yml
summary_line: 1 scheme
tags:
- Company
- B2B
- Data
- Data Enrichment
- Artificial Intelligence
---
