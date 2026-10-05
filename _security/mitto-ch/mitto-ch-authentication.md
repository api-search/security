---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mitto-ch-apis-api-openapi.yml
  format: yaml
  label: Mitto APIs API
  slug: mitto-ch-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitto-ch/refs/heads/main/openapi/mitto-ch-apis-api-openapi.yml
- filename: mitto-ch-autoreplyconfigs-api-openapi.yml
  format: yaml
  label: Mitto Auto Reply Configs API
  slug: mitto-ch-autoreplyconfigs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitto-ch/refs/heads/main/openapi/mitto-ch-autoreplyconfigs-api-openapi.yml
- filename: mitto-ch-customers-api-openapi.yml
  format: yaml
  label: Mitto Customers API
  slug: mitto-ch-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitto-ch/refs/heads/main/openapi/mitto-ch-customers-api-openapi.yml
- filename: mitto-ch-mitto-api-api-openapi.yml
  format: yaml
  label: Mitto Mitto API
  slug: mitto-ch-mitto-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitto-ch/refs/heads/main/openapi/mitto-ch-mitto-api-api-openapi.yml
- filename: mitto-ch-statistic-api-openapi.yml
  format: yaml
  label: Mitto Statistic API
  slug: mitto-ch-statistic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitto-ch/refs/heads/main/openapi/mitto-ch-statistic-api-openapi.yml
- filename: mitto-ch-webhooks-api-openapi.yml
  format: yaml
  label: Mitto Webhooks API
  slug: mitto-ch-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitto-ch/refs/heads/main/openapi/mitto-ch-webhooks-api-openapi.yml
auth_types: []
description: Authentication for Mitto SMS API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mitto Ch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mitto declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Mitto
provider_slug: mitto-ch
scheme_count: 1
schemes:
- evidence: 'To authenticate, you pass your **API key** in the header of the request like this:'
  header: X-Mitto-API-Key
  how_to_obtain: Create an account, then retrieve the API key from Preferences in the Mitto dashboard.
  location: header
  name: X-Mitto-API-Key
  type: apiKey
slug: mitto-ch-authentication
source_filename: mitto-ch-authentication.yml
source_heading: Authentication Profile
source_url: https://documentation.mitto.ch/solutions/editor/preferences/api-keys.md
source_yaml: "generated: '2026-10-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://documentation.mitto.ch/solutions/editor/preferences/api-keys.md\nsources:\n- https://documentation.mitto.ch/solutions/editor/preferences/api-keys.md\n- https://documentation.mitto.ch/apis/sms/authentication.md\n- https://documentation.mitto.ch/getting-started/quickstart.md\n- https://documentation.mitto.ch/getting-started/glossary.md\ndescription: Authentication for Mitto SMS API\nschemes:\n- type: apiKey\n  name: X-Mitto-API-Key\n  evidence: 'To authenticate, you pass your **API key** in the header of the request like this:'\n  location: header\n  header: X-Mitto-API-Key\n  how_to_obtain: Create an account, then retrieve the API key from Preferences in the Mitto dashboard.\ndocs: https://documentation.mitto.ch/solutions/editor/preferences/api-keys.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mitto-ch/refs/heads/main/authentication/mitto-ch-authentication.yml
summary_line: 1 scheme
tags:
- Messaging
- Omnichannel
- Communications
- Enterprise
---
