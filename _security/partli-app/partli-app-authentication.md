---
anonymous_access: false
api_key_in: []
api_specs:
- filename: partli-app-guides-openapi-generated.yml
  format: yaml
  label: Partli guides API
  slug: guides-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/partli-app/openapi/_ae-authored/partli-app-guides-openapi-generated.yml
- filename: partli-app-install-openapi-generated.yml
  format: yaml
  label: Partli install API
  slug: install-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/partli-app/openapi/_ae-authored/partli-app-install-openapi-generated.yml
auth_types: []
description: All Partli REST endpoints accept a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Partli Authentication
name_suffix: Authentication
oauth_flows: []
overview: Partli declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Partli
provider_slug: partli-app
scheme_count: 1
schemes:
- evidence: All Partli REST endpoints accept a Bearer token in the Authorization header.
  header: Authorization
  how_to_obtain: Every Partli workspace gets a Default API key auto‑provisioned on creation; additional keys can be created and revoked from the API keys page in the workspace sidebar. Keys start with pk_live_ and are used as the Bearer token.
  location: header
  name: Bearer
  type: http-bearer
slug: partli-app-authentication
source_filename: partli-app-authentication.yml
source_heading: Authentication Profile
source_url: https://partli.app/docs/api-reference/authentication
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://partli.app/docs/api-reference/authentication\nsources:\n- https://partli.app/docs/api-reference/authentication\n- https://partli.app/docs/install/connect-stripe\n- https://partli.app/docs/quickstart\n- https://partli.app/docs/guides/billing-providers\ndescription: All Partli REST endpoints accept a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: All Partli REST endpoints accept a Bearer token in the Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: Every Partli workspace gets a Default API key auto‑provisioned on creation; additional keys can be created and revoked from the\n    API keys page in the workspace sidebar. Keys start with pk_live_ and are used as the Bearer token.\ndocs: https://partli.app/docs/api-reference/authentication\n"
source_yaml_url: https://artifacts.apis.io/partli-app/authentication/partli-app-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Affiliates
- Software-as-a-Service
- Artificial Intelligence
- Payments
- Partner Programs
---
