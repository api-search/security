---
anonymous_access: false
api_key_in: []
api_specs:
- filename: oceanalt-com-free-api-openapi.yml
  format: yaml
  label: OceanAlt Free API
  slug: oceanalt-com-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oceanalt-com/openapi/oceanalt-com-free-api-openapi.yml
- filename: oceanalt-com-paid-mpp-api-openapi.yml
  format: yaml
  label: OceanAlt paid (mpp) API
  slug: oceanalt-com-paid-mpp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oceanalt-com/openapi/oceanalt-com-paid-mpp-api-openapi.yml
- filename: oceanalt-com-paid-x402-api-openapi.yml
  format: yaml
  label: OceanAlt paid (x402) API
  slug: oceanalt-com-paid-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oceanalt-com/openapi/oceanalt-com-paid-x402-api-openapi.yml
- filename: oceanalt-com-x402-api-openapi.yml
  format: yaml
  label: OceanAlt X402 API
  slug: oceanalt-com-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oceanalt-com/openapi/oceanalt-com-x402-api-openapi.yml
auth_types: []
description: Authentication schemes for OceanAlt API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: OceanAlt Authentication
name_suffix: Authentication
oauth_flows: []
overview: OceanAlt declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: OceanAlt
provider_slug: oceanalt-com
scheme_count: 1
schemes:
- evidence: '带上密钥调用 curl -X POST "https://oceanalt.com/api/decide" \ -H "authorization: Bearer $OCEANALT_API_KEY" \ -H "content-type: application/json" \ -d ''{"to":"0x0000000000000000000000000000000000000000","amountUsdc":25}'''
  header: authorization
  location: header
  name: authorization
  type: apiKey
slug: oceanalt-com-authentication
source_filename: oceanalt-com-authentication.yml
source_heading: Authentication Profile
source_url: https://oceanalt.com/zh/api-keys
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://oceanalt.com/zh/api-keys\nsources:\n- https://oceanalt.com/zh/api-keys\ndescription: Authentication schemes for OceanAlt API\nschemes:\n- type: apiKey\n  name: authorization\n  evidence: '带上密钥调用 curl -X POST \"https://oceanalt.com/api/decide\" \\ -H \"authorization: Bearer $OCEANALT_API_KEY\" \\ -H \"content-type: application/json\"\n    \\ -d ''{\"to\":\"0x0000000000000000000000000000000000000000\",\"amountUsdc\":25}'''\n  location: header\n  header: authorization\ndocs: https://oceanalt.com/zh/api-keys\n"
source_yaml_url: https://artifacts.apis.io/oceanalt-com/authentication/oceanalt-com-authentication.yml
summary_line: 1 scheme
tags:
- Compliance
- Risk Screening
- Investigations
- Developer Tools
---
