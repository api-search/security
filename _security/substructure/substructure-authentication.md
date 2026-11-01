---
anonymous_access: false
api_key_in: []
api_specs:
- filename: substructure-openapi-generated.yml
  format: yaml
  label: Substructure API
  slug: substructure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/substructure/openapi/_ae-authored/substructure-openapi-generated.yml
auth_types: []
description: Authentication schemes for Substructure API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Substructure Authentication
name_suffix: Authentication
oauth_flows: []
overview: Substructure declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Substructure
provider_slug: substructure
scheme_count: 3
schemes:
- evidence: 'A client calls the client API with `Authorization: Bearer <jwt>`.'
  header: Authorization
  how_to_obtain: Create a token through the machine API using an API key (POST /api/machine/client-tokens).
  location: header
  name: Client token
  type: http-bearer
- evidence: Your backend creates these tokens through the machine API, using its own API key.
  header: Authorization
  how_to_obtain: Obtain an API key from the Substructure dashboard or via the cloud provisioning process.
  location: header
  name: API key
  type: apiKey
- evidence: 'X-Substructure-Signature: sha256=<hex HMAC-SHA256 of the body>'
  header: X-Substructure-Signature
  how_to_obtain: Read the signing secret from the deployment (`subs agents secret <id>`) or from the `signing_secret_env` environment variable, then compute the HMAC.
  location: header
  name: Worker request signature
  type: http-header
slug: substructure-authentication
source_filename: substructure-authentication.yml
source_heading: Authentication Profile
source_url: https://substructure.ai/llms.txt/docs/auth.md
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://substructure.ai/llms.txt/docs/auth.md\nsources:\n- https://substructure.ai/llms.txt/docs/auth.md\n- https://substructure.ai/docs/auth\n- https://substructure.ai/llms.txt/docs/quick-start.md\n- https://substructure.ai/llms.txt/docs/quick-start-local.md\ndescription: Authentication schemes for Substructure API\nschemes:\n- type: http-bearer\n  name: Client token\n  evidence: 'A client calls the client API with `Authorization: Bearer <jwt>`.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a token through the machine API using an API key (POST /api/machine/client-tokens).\n- type: apiKey\n  name: API key\n  evidence: Your backend creates these tokens through the machine API, using its own API key.\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain an API key from the Substructure dashboard or via the cloud provisioning process.\n- type:\
  \ http-header\n  name: Worker request signature\n  evidence: 'X-Substructure-Signature: sha256=<hex HMAC-SHA256 of the body>'\n  location: header\n  header: X-Substructure-Signature\n  how_to_obtain: Read the signing secret from the deployment (`subs agents secret <id>`) or from the `signing_secret_env` environment variable,\n    then compute the HMAC.\ndocs: https://substructure.ai/llms.txt/docs/auth.md\n"
source_yaml_url: https://artifacts.apis.io/substructure/authentication/substructure-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Artificial Intelligence
- Agents
- Cloud-Native
- Automation
---
