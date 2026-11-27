---
anonymous_access: false
api_key_in: []
api_specs:
- filename: oracleinsight-xyz-mcp-api-openapi.yml
  format: yaml
  label: Insight MCP API
  slug: oracleinsight-xyz-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oracleinsight-xyz/openapi/oracleinsight-xyz-mcp-api-openapi.yml
- filename: oracleinsight-xyz-safety-api-openapi.yml
  format: yaml
  label: Insight Safety API
  slug: oracleinsight-xyz-safety-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oracleinsight-xyz/openapi/oracleinsight-xyz-safety-api-openapi.yml
auth_types: []
description: Authentication methods published on Insight documentation
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Insight Authentication
name_suffix: Authentication
oauth_flows: []
overview: Insight declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Insight
provider_slug: oracleinsight-xyz
scheme_count: 1
schemes:
- evidence: Use X-API-Key on metered endpoints.
  header: X-API-Key
  how_to_obtain: Get an API Key — Create one in Settings. It's shown only once, so store it securely.
  location: header
  name: X-API-Key
  type: apiKey
slug: oracleinsight-xyz-authentication
source_filename: oracleinsight-xyz-authentication.yml
source_heading: Authentication Profile
source_url: https://www.oracleinsight.xyz/docs/x402
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.oracleinsight.xyz/docs/x402\nsources:\n- https://www.oracleinsight.xyz/docs/x402\n- https://www.oracleinsight.xyz/docs/api\ndescription: Authentication methods published on Insight documentation\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: Use X-API-Key on metered endpoints.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Get an API Key — Create one in Settings. It's shown only once, so store it securely.\nnote: External v1 endpoints accept API keys only.\ndocs: https://www.oracleinsight.xyz/docs/x402\n"
source_yaml_url: https://artifacts.apis.io/oracleinsight-xyz/authentication/oracleinsight-xyz-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Oracle
- Risk Intelligence
- DeFi
- Data Integrity
---
