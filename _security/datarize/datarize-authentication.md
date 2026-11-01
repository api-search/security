---
anonymous_access: false
api_key_in: []
api_specs:
- filename: datarize-openapi-generated.yml
  format: yaml
  label: Datarize API
  slug: datarize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datarize/openapi/_ae-authored/datarize-openapi-generated.yml
auth_types: []
description: Authentication schemes for Datarize API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Datarize Authentication
name_suffix: Authentication
oauth_flows: []
overview: Datarize declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Datarize
provider_slug: datarize
scheme_count: 1
schemes:
- evidence: 키는 서버에만 보관하고 Authorization 헤더로 전달합니다.
  header: Authorization
  how_to_obtain: 시험 키( dtr_test_v1_ )와 실제 키( dtr_live_v1_ )
  location: header
  name: API Key
  type: apiKey
slug: datarize-authentication
source_filename: datarize-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.datarize.ai/getting-started/
source_yaml: "generated: '2026-10-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.datarize.ai/getting-started/\nsources:\n- https://developer.datarize.ai/getting-started/\ndescription: Authentication schemes for Datarize API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 키는 서버에만 보관하고 Authorization 헤더로 전달합니다.\n  location: header\n  header: Authorization\n  how_to_obtain: 시험 키( dtr_test_v1_ )와 실제 키( dtr_live_v1_ )\ndocs: https://developer.datarize.ai/getting-started/\n"
source_yaml_url: https://artifacts.apis.io/datarize/authentication/datarize-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Data Integration
- Analytics
- API Platform
- Enterprise
---
