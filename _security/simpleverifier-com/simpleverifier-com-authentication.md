---
anonymous_access: false
api_key_in: []
auth_types: []
description: SimpleVerifier uses an API key provided as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Simpleverifier Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: SimpleVerifier declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: SimpleVerifier
provider_slug: simpleverifier-com
scheme_count: 1
schemes:
- evidence: Create an API key, then send GET or POST https://simpleverifier.com/api/v1/verify with the address as email and the key as a Bearer token.
  header: Authorization
  how_to_obtain: Create one on the API keys page; the key starts with sv_live_ and is shown once.
  location: header
  name: Bearer token
  type: http-bearer
slug: simpleverifier-com-authentication
source_filename: simpleverifier-com-authentication.yml
source_heading: Authentication Profile
source_url: https://simpleverifier.com/docs/quickstart
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://simpleverifier.com/docs/quickstart\nsources:\n- https://simpleverifier.com/docs/quickstart\ndescription: SimpleVerifier uses an API key provided as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: Create an API key, then send GET or POST https://simpleverifier.com/api/v1/verify with the address as email and the key as a Bearer\n    token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create one on the API keys page; the key starts with sv_live_ and is shown once.\ndocs: https://simpleverifier.com/docs/quickstart\n"
source_yaml_url: https://artifacts.apis.io/simpleverifier-com/authentication/simpleverifier-com-authentication.yml
summary_line: 1 scheme
tags:
- Email Verification
- Software-as-a-Service
- BulkTools
- Security
---
