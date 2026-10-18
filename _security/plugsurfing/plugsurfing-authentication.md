---
anonymous_access: false
api_key_in: []
api_specs:
- filename: plugsurfing-charging-key-orders-api-openapi.yml
  format: yaml
  label: Plugsurfing Charging Key Orders API
  slug: plugsurfing-charging-key-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-charging-key-orders-api-openapi.yml
- filename: plugsurfing-charging-keys-api-openapi.yml
  format: yaml
  label: Plugsurfing Charging Keys API
  slug: plugsurfing-charging-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-charging-keys-api-openapi.yml
- filename: plugsurfing-drive-api-api-openapi.yml
  format: yaml
  label: Plugsurfing Drive API
  slug: plugsurfing-drive-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-drive-api-api-openapi.yml
- filename: plugsurfing-emp-charging-keys-api-openapi.yml
  format: yaml
  label: Plugsurfing EMP Charging Keys API
  slug: plugsurfing-emp-charging-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-emp-charging-keys-api-openapi.yml
- filename: plugsurfing-emp-fleets-api-openapi.yml
  format: yaml
  label: Plugsurfing EMP Fleets API
  slug: plugsurfing-emp-fleets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-emp-fleets-api-openapi.yml
- filename: plugsurfing-emp-geosearch-api-openapi.yml
  format: yaml
  label: Plugsurfing EMP Geosearch API
  slug: plugsurfing-emp-geosearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-emp-geosearch-api-openapi.yml
- filename: plugsurfing-emp-orders-api-openapi.yml
  format: yaml
  label: Plugsurfing EMP Orders API
  slug: plugsurfing-emp-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-emp-orders-api-openapi.yml
- filename: plugsurfing-emp-sessions-api-openapi.yml
  format: yaml
  label: Plugsurfing EMP Sessions API
  slug: plugsurfing-emp-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-emp-sessions-api-openapi.yml
- filename: plugsurfing-geosearch-api-openapi.yml
  format: yaml
  label: Plugsurfing Geosearch API
  slug: plugsurfing-geosearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-geosearch-api-openapi.yml
- filename: plugsurfing-payment-options-api-openapi.yml
  format: yaml
  label: Plugsurfing Payment Options API
  slug: plugsurfing-payment-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-payment-options-api-openapi.yml
- filename: plugsurfing-remote-charging-api-openapi.yml
  format: yaml
  label: Plugsurfing Remote Charging API
  slug: plugsurfing-remote-charging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-remote-charging-api-openapi.yml
- filename: plugsurfing-sessions-api-openapi.yml
  format: yaml
  label: Plugsurfing Sessions API
  slug: plugsurfing-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-sessions-api-openapi.yml
- filename: plugsurfing-user-groups-api-openapi.yml
  format: yaml
  label: Plugsurfing User Groups API
  slug: plugsurfing-user-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-user-groups-api-openapi.yml
- filename: plugsurfing-users-api-openapi.yml
  format: yaml
  label: Plugsurfing Users API
  slug: plugsurfing-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-users-api-openapi.yml
- filename: plugsurfing-vouchers-api-openapi.yml
  format: yaml
  label: Plugsurfing Vouchers API
  slug: plugsurfing-vouchers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-vouchers-api-openapi.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Plugsurfing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Plugsurfing declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Plugsurfing
provider_slug: plugsurfing
scheme_count: 1
schemes:
- evidence: Every API request must include the API key in the `X-API-Key` header.
  header: X-API-Key
  how_to_obtain: You can obtain the API key from the Control Panel for both stage and production environments (ask your CSM for access).
  location: header
  name: X-API-Key
  type: apiKey
slug: plugsurfing-authentication
source_filename: plugsurfing-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.plugsurfing.com/docs/drive-api/authorization.md
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.plugsurfing.com/docs/drive-api/authorization.md\nsources:\n- https://developer.plugsurfing.com/docs/drive-api/authorization.md\n- https://developer.plugsurfing.com/reference/getStripePublishableApiKey.md\n- https://developer.plugsurfing.com/docs/drive-api/authorization\n- https://developer.plugsurfing.com/docs/roam-ocpi/credentials-module.md\ndescription: Authentication\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: Every API request must include the API key in the `X-API-Key` header.\n  location: header\n  header: X-API-Key\n  how_to_obtain: You can obtain the API key from the Control Panel for both stage and production environments (ask your CSM for access).\ndocs: https://developer.plugsurfing.com/docs/drive-api/authorization.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/authentication/plugsurfing-authentication.yml
summary_line: 1 scheme
tags:
- Company
- EVCharging
- Roaming
- Europe
---
