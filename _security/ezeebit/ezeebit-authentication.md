---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ezeebit-openapi-generated.yml
  format: yaml
  label: Ezeebit API
  slug: ezeebit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ezeebit/openapi/_ae-authored/ezeebit-openapi-generated.yml
auth_types: []
description: Ezeebit uses a custom HMAC‑based authentication scheme.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ezeebit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ezeebit declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Ezeebit
provider_slug: ezeebit
scheme_count: 1
schemes:
- evidence: The **API key** will be visible on the portal, but the **Secret key** will not be displayed again.
  header: Ezeebit-Certificate-SN
  how_to_obtain: Create an API key and Secret key in the merchant portal (https://merchant.ezeebit.com/#/login) via the API Management section. The API key is shown; the Secret key must be saved immediately as it cannot be retrieved later.
  location: header
  name: Ezeebit HMAC
  type: hmac
slug: ezeebit-authentication
source_filename: ezeebit-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.ezeebit.com/api-authentication.md
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.ezeebit.com/api-authentication.md\nsources:\n- https://docs.ezeebit.com/api-authentication.md\ndescription: Ezeebit uses a custom HMAC‑based authentication scheme.\nschemes:\n- type: hmac\n  name: Ezeebit HMAC\n  evidence: The **API key** will be visible on the portal, but the **Secret key** will not be displayed again.\n  location: header\n  header: Ezeebit-Certificate-SN\n  how_to_obtain: Create an API key and Secret key in the merchant portal (https://merchant.ezeebit.com/#/login) via the API Management section.\n    The API key is shown; the Secret key must be saved immediately as it cannot be retrieved later.\ndocs: https://docs.ezeebit.com/api-authentication.md\n"
source_yaml_url: https://artifacts.apis.io/ezeebit/authentication/ezeebit-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Payments
- Cryptocurrency
- Africa
- ePOS
---
