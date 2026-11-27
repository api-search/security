---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fastinsight-ai-openapi-generated.yml
  format: yaml
  label: Fast Insight API
  slug: fastinsight-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastinsight-ai/openapi/_ae-authored/fastinsight-ai-openapi-generated.yml
auth_types: []
description: Fast Insight MCP uses OAuth for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fast Insight Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fast Insight declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Fast Insight
provider_slug: fastinsight-ai
scheme_count: 1
schemes:
- authorize_url: https://fastinsight.ai/api/oauth/authorize
  evidence: MCP クライアントがサーバーから OAuth の情報を自動で取得します。
  flows:
  - authorization_code
  how_to_obtain: Log in to Fast Insight in a browser and grant permission when prompted.
  name: OAuth
  type: oauth2
slug: fastinsight-ai-authentication
source_filename: fastinsight-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://fastinsight.ai/docs/mcp-connect?lang=ja
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://fastinsight.ai/docs/mcp-connect?lang=ja\nsources:\n- https://fastinsight.ai/docs/mcp-connect?lang=ja\ndescription: Fast Insight MCP uses OAuth for authentication.\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: MCP クライアントがサーバーから OAuth の情報を自動で取得します。\n  flows:\n  - authorization_code\n  authorize_url: https://fastinsight.ai/api/oauth/authorize\n  how_to_obtain: Log in to Fast Insight in a browser and grant permission when prompted.\ndocs: https://fastinsight.ai/docs/mcp-connect?lang=ja\n"
source_yaml_url: https://artifacts.apis.io/fastinsight-ai/authentication/fastinsight-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Market Research
- Qualitative Insights
- Global Panel
- Japanese Market
---
