---
anonymous_access: false
api_key_in: []
api_specs:
- filename: loqate-plants-api-openapi.yml
  format: yaml
  label: Loqate Plants API
  slug: loqate-plants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loqate/refs/heads/main/openapi/loqate-plants-api-openapi.yml
auth_types: []
description: All Loqate services require a valid and active API key for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Loqate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Loqate declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Loqate
provider_slug: loqate
scheme_count: 1
schemes:
- evidence: All Loqate services require a valid and active API key for authentication.
  how_to_obtain: Create an API key in the Loqate account setup page.
  location: query
  name: Key
  type: apiKey
slug: loqate-authentication
source_filename: loqate-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.loqate.com/loqate-basics/create-an-api-key.md
source_yaml: "generated: '2026-10-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.loqate.com/loqate-basics/create-an-api-key.md\nsources:\n- https://docs.loqate.com/loqate-basics/create-an-api-key.md\n- https://docs.loqate.com/getting-started/country-improvement-program.md\n- https://docs.loqate.com/our-services/address-capture/address-capture-quick-start.md\n- https://docs.loqate.com/our-services/tag-setup-guide.md\ndescription: All Loqate services require a valid and active API key for authentication.\nschemes:\n- type: apiKey\n  name: Key\n  evidence: All Loqate services require a valid and active API key for authentication.\n  location: query\n  how_to_obtain: Create an API key in the Loqate account setup page.\ndocs: https://docs.loqate.com/loqate-basics/create-an-api-key.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loqate/refs/heads/main/authentication/loqate-authentication.yml
summary_line: 1 scheme
tags:
- Address Validation
- Data Quality
- Email Verification
- Phone Validation
- Retail
- Fintech
- Logistics
---
