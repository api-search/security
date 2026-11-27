---
anonymous_access: false
api_key_in: []
api_specs:
- filename: keirolabs-openapi-generated.yml
  format: yaml
  label: Keirolabs API
  slug: keirolabs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keirolabs/openapi/_ae-authored/keirolabs-openapi-generated.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Keirolabs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keirolabs declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Keirolabs
provider_slug: keirolabs
scheme_count: 1
schemes:
- evidence: Send your API key as a Bearer token.
  header: Authorization
  how_to_obtain: Create and revoke keys in Dashboard → API Keys; a key is shown once when you create it.
  location: header
  name: Bearer token
  type: http-bearer
slug: keirolabs-authentication
source_filename: keirolabs-authentication.yml
source_heading: Authentication Profile
source_url: https://platform.keirolabs.cloud/register?src=docs
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://platform.keirolabs.cloud/register?src=docs\nsources:\n- https://platform.keirolabs.cloud/register?src=docs\n- https://docs.keirolabs.cloud/authentication\n- https://platform.keirolabs.cloud/register?utm_source=keirolabs&utm_medium=home&utm_content=hero\n- https://docs.keirolabs.cloud/quickstart\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: Send your API key as a Bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create and revoke keys in Dashboard → API Keys; a key is shown once when you create it.\ndocs: https://platform.keirolabs.cloud/register?src=docs\n"
source_yaml_url: https://artifacts.apis.io/keirolabs/authentication/keirolabs-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Search
- Data Extraction
- Web API
- Software-as-a-Service
---
