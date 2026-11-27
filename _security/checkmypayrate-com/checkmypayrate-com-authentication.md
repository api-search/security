---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: CheckMyPayRate Authentication
name_suffix: Authentication
oauth_flows: []
overview: CheckMyPayRate declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CheckMyPayRate
provider_slug: checkmypayrate-com
scheme_count: 1
schemes:
- applies_to:
  - https://checkmypayrate.com/mcp
  - https://checkmypayrate.com/api/public/dataset/csv
  - https://checkmypayrate.com/api/public/dataset/json
  evidence: '- **Authentication:** none required'
  name: none
  type: none
slug: checkmypayrate-com-authentication
source_filename: checkmypayrate-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://github.com/markopints34-tech/checkmypayrate/blob/main/README.md\nnote: No OpenAPI exists. The README of the GitHub repo markopints34-tech/checkmypayrate (homepage set to https://checkmypayrate.com, describes this site's dataset and MCP server; not linked from the site itself) states the MCP endpoint needs no authentication. The dataset downloads at /api/public/dataset/{csv,json} answered 200 to an unauthenticated GET on 2026-11-03.\nschemes:\n- name: none\n  type: none\n  applies_to:\n  - https://checkmypayrate.com/mcp\n  - https://checkmypayrate.com/api/public/dataset/csv\n  - https://checkmypayrate.com/api/public/dataset/json\n  evidence: '- **Authentication:** none required'\n"
source_yaml_url: https://artifacts.apis.io/checkmypayrate-com/authentication/checkmypayrate-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Salary
- Compensation
- Benchmarks
- Labor Market Data
- Open Data
- Calculators
---
