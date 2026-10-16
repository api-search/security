---
anonymous_access: false
api_key_in: []
api_specs:
- filename: datia-openapi-generated.yml
  format: yaml
  label: Datia API
  slug: datia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datia/refs/heads/main/openapi/_ae-authored/datia-openapi-generated.yml
auth_types: []
description: Datia uses a simple API key authentication scheme.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Datia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Datia declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Datia
provider_slug: datia
scheme_count: 1
schemes:
- evidence: Send your API key in the x-api-key header.
  header: x-api-key
  how_to_obtain: Ask your Connect Earth contact or customers@connect.earth for a key.
  location: header
  name: API Key
  type: apiKey
slug: datia-authentication
source_filename: datia-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.datia.app/docs/authentication/
source_yaml: "generated: '2026-10-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.datia.app/docs/authentication/\nsources:\n- https://docs.datia.app/docs/authentication/\n- https://docs.datia.app/docs/authentication/\n- https://docs.datia.app/docs/quickstart/\n- https://docs.datia.app/docs/quickstart/\ndescription: Datia uses a simple API key authentication scheme.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Send your API key in the x-api-key header.\n  location: header\n  header: x-api-key\n  how_to_obtain: Ask your Connect Earth contact or customers@connect.earth for a key.\ndocs: https://docs.datia.app/docs/authentication/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datia/refs/heads/main/authentication/datia-authentication.yml
summary_line: 1 scheme
tags:
- Sustainable Finance
- ESG
- Data Platform
- API
- Finance
---
