---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for SanctionsKit API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Sanctionskit Authentication
name_suffix: Authentication
oauth_flows: []
overview: SanctionsKit declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: SanctionsKit
provider_slug: sanctionskit
scheme_count: 1
schemes:
- evidence: 'Transport Bearer token Send credentials in the Authorization header. Send machine credentials in a header API clients send Authorization: Bearer followed by the secret.'
  header: Authorization
  how_to_obtain: Get your free API key from the dashboard (sandbox keys start with sk_test_, production keys start with sk_live_).
  location: header
  name: Bearer
  scopes:
  - sources:read
  - screenings:write
  - results:read
  - batches:write
  - monitors:write
  - usage:read
  - webhooks:write
  type: http-bearer
slug: sanctionskit-authentication
source_filename: sanctionskit-authentication.yml
source_heading: Authentication Profile
source_url: https://www.sanctionskit.com/docs/authentication
source_yaml: "generated: '2026-10-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.sanctionskit.com/docs/authentication\nsources:\n- https://www.sanctionskit.com/docs/authentication\n- https://www.sanctionskit.com/docs/api-reference/endpoints/post-uploads\n- https://www.sanctionskit.com/docs/api-reference/endpoints/post-webhooks\n- https://www.sanctionskit.com/docs/api-reference/schemas/upload-token-request\ndescription: Authentication schemes for SanctionsKit API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Transport Bearer token Send credentials in the Authorization header. Send machine credentials in a header API clients send Authorization:\n    Bearer followed by the secret.'\n  location: header\n  header: Authorization\n  scopes:\n  - sources:read\n  - screenings:write\n  - results:read\n  - batches:write\n  - monitors:write\n  - usage:read\n  - webhooks:write\n  how_to_obtain: Get your free API key from the dashboard (sandbox\
  \ keys start with sk_test_, production keys start with sk_live_).\nnote: Human sessions use signed‑in browser sessions and are not an API authentication scheme.\ndocs: https://www.sanctionskit.com/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sanctionskit/refs/heads/main/authentication/sanctionskit-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Sanctions
- Compliance
- Screening
- Fintech
---
