---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication uses an API key sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fortytwo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fortytwo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Fortytwo
provider_slug: fortytwo-network
scheme_count: 1
schemes:
- evidence: '-H "Authorization: Bearer $FORTYTWO_API_KEY"'
  header: Authorization
  how_to_obtain: Create an API key in the Fortytwo platform (see Quickstart).
  location: header
  name: Bearer
  type: http-bearer
slug: fortytwo-network-authentication
source_filename: fortytwo-network-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.fortytwo.network/docs/quickstart.md
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.fortytwo.network/docs/quickstart.md\nsources:\n- https://docs.fortytwo.network/docs/quickstart.md\n- https://docs.fortytwo.network/docs/quickstart\ndescription: Authentication uses an API key sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: '-H \"Authorization: Bearer $FORTYTWO_API_KEY\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the Fortytwo platform (see Quickstart).\ndocs: https://docs.fortytwo.network/docs/quickstart.md\n"
source_yaml_url: https://artifacts.apis.io/fortytwo-network/authentication/fortytwo-network-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Platform
- Open Source
---
