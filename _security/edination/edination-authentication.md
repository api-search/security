---
anonymous_access: false
api_key_in: []
api_specs:
- filename: edination-openapi-generated.yml
  format: yaml
  label: EdiNation API
  slug: edination-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edination/openapi/_ae-authored/edination-openapi-generated.yml
auth_types: []
description: Authentication schemes for EdiNation products
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Edination Authentication
name_suffix: Authentication
oauth_flows: []
overview: EdiNation declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: EdiNation
provider_slug: edination
scheme_count: 1
schemes:
- evidence: Send the serial on every request as the Ocp-Apim-Subscription-Key header.
  header: Ocp-Apim-Subscription-Key
  location: header
  name: Ocp-Apim-Subscription-Key
  type: apiKey
slug: edination-authentication
source_filename: edination-authentication.yml
source_heading: Authentication Profile
source_url: https://www.edifabric.com/docs/edifabric-net/licensing.html
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.edifabric.com/docs/edifabric-net/licensing.html\nsources:\n- https://www.edifabric.com/docs/edifabric-net/licensing.html\n- https://www.edifabric.com/docs/getting-started/introduction.html\n- https://www.edifabric.com/docs/getting-started/your-account.html\n- https://www.edifabric.com/docs/getting-started/convert-between-edi-and-json.html\ndescription: Authentication schemes for EdiNation products\nschemes:\n- type: apiKey\n  name: Ocp-Apim-Subscription-Key\n  evidence: Send the serial on every request as the Ocp-Apim-Subscription-Key header.\n  location: header\n  header: Ocp-Apim-Subscription-Key\ndocs: https://www.edifabric.com/docs/edifabric-net/licensing.html\n"
source_yaml_url: https://artifacts.apis.io/edination/authentication/edination-authentication.yml
summary_line: 1 scheme
tags:
- Company
- EDI
- Healthcare
- Validation
- Open Source
---
