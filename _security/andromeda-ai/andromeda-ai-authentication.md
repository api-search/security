---
anonymous_access: false
api_key_in: []
api_specs:
- filename: andromeda-ai-openapi-generated.yml
  format: yaml
  label: Andromeda API
  slug: andromeda-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/andromeda-ai/openapi/_ae-authored/andromeda-ai-openapi-generated.yml
auth_types: []
description: Authentication is performed with an OpenID Connect (OIDC) bearer token attached to each request.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Andromeda Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Andromeda declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Andromeda
provider_slug: andromeda-ai
scheme_count: 1
schemes:
- evidence: 'Send the access token in the `Authorization` header:'
  header: Authorization
  how_to_obtain: Via the Andromeda CLI device login (`andromeda auth login`) or by using your own OpenID Connect client to obtain an access token with the required audiences and scopes.
  location: header
  name: OIDC Bearer Token
  type: http-bearer
slug: andromeda-ai-authentication
source_filename: andromeda-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.andromeda.ai/clusters/authentication.md
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.andromeda.ai/clusters/authentication.md\nsources:\n- https://docs.andromeda.ai/clusters/authentication.md\n- https://docs.andromeda.ai/clusters/quickstart.md\ndescription: Authentication is performed with an OpenID Connect (OIDC) bearer token attached to each request.\nschemes:\n- type: http-bearer\n  name: OIDC Bearer Token\n  evidence: 'Send the access token in the `Authorization` header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Via the Andromeda CLI device login (`andromeda auth login`) or by using your own OpenID Connect client to obtain an access token\n    with the required audiences and scopes.\nnote: The documentation does not list any API‑key, client‑credentials, authorization‑code, or other OAuth flows, nor does it provide explicit\n  token or authorize URLs; therefore those fields are left null or empty.\ndocs: https://docs.andromeda.ai/clusters/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/andromeda-ai/authentication/andromeda-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Cloud
- Platform
- Machine-Learning
- Enterprise
---
