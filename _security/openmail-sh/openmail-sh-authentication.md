---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openmail-sh-attachments-api-openapi.yml
  format: yaml
  label: openmail-sh Attachments API
  slug: openmail-sh-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmail-sh/openapi/openmail-sh-attachments-api-openapi.yml
- filename: openmail-sh-domains-api-openapi.yml
  format: yaml
  label: openmail-sh Domains API
  slug: openmail-sh-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmail-sh/openapi/openmail-sh-domains-api-openapi.yml
- filename: openmail-sh-feedback-api-openapi.yml
  format: yaml
  label: openmail-sh Feedback API
  slug: openmail-sh-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmail-sh/openapi/openmail-sh-feedback-api-openapi.yml
- filename: openmail-sh-inboxes-api-openapi.yml
  format: yaml
  label: openmail-sh Inboxes API
  slug: openmail-sh-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmail-sh/openapi/openmail-sh-inboxes-api-openapi.yml
- filename: openmail-sh-limits-api-openapi.yml
  format: yaml
  label: openmail-sh Limits API
  slug: openmail-sh-limits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmail-sh/openapi/openmail-sh-limits-api-openapi.yml
- filename: openmail-sh-messages-api-openapi.yml
  format: yaml
  label: openmail-sh Messages API
  slug: openmail-sh-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmail-sh/openapi/openmail-sh-messages-api-openapi.yml
- filename: openmail-sh-owned-domains-api-openapi.yml
  format: yaml
  label: openmail-sh Owned Domains API
  slug: openmail-sh-owned-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmail-sh/openapi/openmail-sh-owned-domains-api-openapi.yml
- filename: openmail-sh-pods-api-openapi.yml
  format: yaml
  label: openmail-sh Pods API
  slug: openmail-sh-pods-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmail-sh/openapi/openmail-sh-pods-api-openapi.yml
- filename: openmail-sh-policy-api-openapi.yml
  format: yaml
  label: openmail-sh Policy API
  slug: openmail-sh-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmail-sh/openapi/openmail-sh-policy-api-openapi.yml
- filename: openmail-sh-threads-api-openapi.yml
  format: yaml
  label: openmail-sh Threads API
  slug: openmail-sh-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmail-sh/openapi/openmail-sh-threads-api-openapi.yml
auth_types: []
description: Authentication methods published for OpenMail
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Openmail Sh Authentication
name_suffix: Authentication
oauth_flows: []
overview: openmail-sh declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: openmail-sh
provider_slug: openmail-sh
scheme_count: 1
schemes:
- evidence: OpenMail uses API key authentication. Pass your secret key as a Bearer token in the Authorization header on every request to the REST API.
  header: Authorization
  how_to_obtain: Sign up at the Dashboard, complete the setup wizard, and copy your API key (prefixed with `om_`). Scoped keys are minted via POST /v1/inboxes/{id}/api-keys or POST /v1/pods/{id}/api-keys.
  location: header
  name: Bearer
  type: http-bearer
slug: openmail-sh-authentication
source_filename: openmail-sh-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.openmail.sh/best-practices/api-key-scopes.md
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.openmail.sh/best-practices/api-key-scopes.md\nsources:\n- https://docs.openmail.sh/best-practices/api-key-scopes.md\n- https://docs.openmail.sh/api-reference/authentication.md\n- https://docs.openmail.sh/api-reference/pods/create-pod-api-key.md\n- https://docs.openmail.sh/api-reference/pods/list-pod-api-keys.md\ndescription: Authentication methods published for OpenMail\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: OpenMail uses API key authentication. Pass your secret key as a Bearer token in the Authorization header on every request to the REST\n    API.\n  location: header\n  header: Authorization\n  how_to_obtain: Sign up at the Dashboard, complete the setup wizard, and copy your API key (prefixed with `om_`). Scoped keys are minted via\n    POST /v1/inboxes/{id}/api-keys or POST /v1/pods/{id}/api-keys.\nnote: No OAuth2, apiKey, or other schemes are\
  \ documented.\ndocs: https://docs.openmail.sh/best-practices/api-key-scopes.md\n"
source_yaml_url: https://artifacts.apis.io/openmail-sh/authentication/openmail-sh-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Email
- API
- AI
- Developer
---
