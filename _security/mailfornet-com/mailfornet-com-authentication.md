---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mailfornet-com-account-api-openapi.yml
  format: yaml
  label: Mailfornet Account API
  slug: mailfornet-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfornet-com/openapi/mailfornet-com-account-api-openapi.yml
- filename: mailfornet-com-inboxes-api-openapi.yml
  format: yaml
  label: Mailfornet Inboxes API
  slug: mailfornet-com-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfornet-com/openapi/mailfornet-com-inboxes-api-openapi.yml
- filename: mailfornet-com-messages-api-openapi.yml
  format: yaml
  label: Mailfornet Messages API
  slug: mailfornet-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfornet-com/openapi/mailfornet-com-messages-api-openapi.yml
- filename: mailfornet-com-webhooks-api-openapi.yml
  format: yaml
  label: Mailfornet Webhooks API
  slug: mailfornet-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfornet-com/openapi/mailfornet-com-webhooks-api-openapi.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mailfornet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mailfornet declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Mailfornet
provider_slug: mailfornet-com
scheme_count: 1
schemes:
- evidence: 'Every request carries your key as a bearer token: Authorization: Bearer mf_live_...'
  header: Authorization
  how_to_obtain: Create keys in your account. A key is shown once, when you create it.
  location: header
  name: Bearer
  type: http-bearer
slug: mailfornet-com-authentication
source_filename: mailfornet-com-authentication.yml
source_heading: Authentication Profile
source_url: https://mailfornet.com/developers/signup
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mailfornet.com/developers/signup\nsources:\n- https://mailfornet.com/developers/signup\n- https://mailfornet.com/api\n- https://mailfornet.com/developers/quickstart\n- https://mailfornet.com/developers/mcp\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Every request carries your key as a bearer token: Authorization: Bearer mf_live_...'\n  location: header\n  header: Authorization\n  how_to_obtain: Create keys in your account. A key is shown once, when you create it.\ndocs: https://mailfornet.com/developers/signup\n"
source_yaml_url: https://artifacts.apis.io/mailfornet-com/authentication/mailfornet-com-authentication.yml
summary_line: 1 scheme
tags:
- temporary-email
- Disposable Email
- Email Verification
- Privacy
- Developer API
---
