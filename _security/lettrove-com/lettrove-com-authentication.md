---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lettrove-com-server-api-api-openapi.yml
  format: yaml
  label: Lettrove Server API
  slug: lettrove-com-server-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lettrove-com/openapi/lettrove-com-server-api-api-openapi.yml
- filename: lettrove-com-webhooks-api-openapi.yml
  format: yaml
  label: Lettrove Webhooks API
  slug: lettrove-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lettrove-com/openapi/lettrove-com-webhooks-api-openapi.yml
auth_types: []
description: Clients obtain a secret key from Lettrove Settings → Embed and use it as a Bearer token in the Authorization header when calling the token endpoint.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Lettrove Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lettrove declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Lettrove
provider_slug: lettrove-com
scheme_count: 1
schemes:
- evidence: 'Authorization: Bearer lt_sk_test_…'
  header: Authorization
  how_to_obtain: Copy the secret key (lt_sk_…) from the project’s Settings → Embed page; it is used only on the server.
  location: header
  name: Bearer
  type: http-bearer
slug: lettrove-com-authentication
source_filename: lettrove-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.lettrove.com/docs/server/tokens.md
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.lettrove.com/docs/server/tokens.md\nsources:\n- https://docs.lettrove.com/docs/server/tokens.md\n- https://docs.lettrove.com/docs/server/tokens\n- https://docs.lettrove.com/docs/1.0/server/tokens\n- https://docs.lettrove.com/docs/get-started/quickstart.md\ndescription: Clients obtain a secret key from Lettrove Settings → Embed and use it as a Bearer token in the Authorization header when calling\n  the token endpoint.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authorization: Bearer lt_sk_test_…'\n  location: header\n  header: Authorization\n  how_to_obtain: Copy the secret key (lt_sk_…) from the project’s Settings → Embed page; it is used only on the server.\ndocs: https://docs.lettrove.com/docs/server/tokens.md\n"
source_yaml_url: https://artifacts.apis.io/lettrove-com/authentication/lettrove-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Email
- Marketing
- Collaboration
---
