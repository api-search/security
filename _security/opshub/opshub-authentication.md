---
anonymous_access: false
api_key_in: []
api_specs:
- filename: opshub-openapi-generated.yml
  format: yaml
  label: OpsHub API
  slug: opshub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opshub/openapi/_ae-authored/opshub-openapi-generated.yml
auth_types: []
description: OpsHub supports API Key authentication for its Admin and MCP APIs.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Opshub Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpsHub declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: OpsHub
provider_slug: opshub
scheme_count: 1
schemes:
- evidence: 'Pass the key in one of the following request headers:


    ```

    x-api-key: <api-key>

    ```'
  header: x-api-key
  how_to_obtain: Create an API Key in the OpsHub UI under Administration → API key; the key value is shown once after creation.
  location: header
  name: API Key (x-api-key header)
  type: apiKey
slug: opshub-authentication
source_filename: opshub-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.opshub.com/manage/administrator/api-key-management.md
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.opshub.com/manage/administrator/api-key-management.md\nsources:\n- https://docs.opshub.com/manage/administrator/api-key-management.md\n- https://docs.opshub.com/manage/advanced-utilities/switching-to-windows-authentication-mode-for-mssql-server.md\n- https://docs.opshub.com/connectors/ibm-rational-doors-next-generation/ibm-rational-doors-next-oauth-generation.md\n- https://docs.opshub.com/mbse-connector-sdk-index/mbse-sdk-connector-apis/authentication-apis.md\ndescription: OpsHub supports API Key authentication for its Admin and MCP APIs.\nschemes:\n- type: apiKey\n  name: API Key (x-api-key header)\n  evidence: 'Pass the key in one of the following request headers:\n\n\n    ```\n\n    x-api-key: <api-key>\n\n    ```'\n  location: header\n  header: x-api-key\n  how_to_obtain: Create an API Key in the OpsHub UI under Administration → API key; the key value is shown once\
  \ after creation.\nnote: OAuth 1.0 token generation for IBM DOORS Next is described, but it is not an authentication scheme for OpsHub APIs themselves. 1 extracted\n  row(s) were dropped because their quote was not on the page.\ndocs: https://docs.opshub.com/manage/administrator/api-key-management.md\n"
source_yaml_url: https://artifacts.apis.io/opshub/authentication/opshub-authentication.yml
summary_line: 1 scheme
tags:
- Integration
- Migration
- ALM
- ITSM
- CRM
- DevOps
- Enterprise
---
