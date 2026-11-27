---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mostlyright-md-guides-openapi-generated.yml
  format: yaml
  label: Mostly Right guides API
  slug: guides-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mostlyright-md/openapi/_ae-authored/mostlyright-md-guides-openapi-generated.yml
- filename: mostlyright-md-reference-openapi-generated.yml
  format: yaml
  label: Mostly Right Overview API
  slug: reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mostlyright-md/openapi/_ae-authored/mostlyright-md-reference-openapi-generated.yml
- filename: mostlyright-md-start-openapi-generated.yml
  format: yaml
  label: Mostly Right start API
  slug: start-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mostlyright-md/openapi/_ae-authored/mostlyright-md-start-openapi-generated.yml
auth_types: []
description: Authentication methods described for Mostly Right
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Mostly Right Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mostly Right declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Mostly Right
provider_slug: mostlyright-md
scheme_count: 2
schemes:
- evidence: mr-data login signs this machine in to the Mostly Right cloud. It prints a short code and an approval address on stderr and opens a browser. On approval it stores a durable device credential at ~/.mostlyright/credentials , mode 0600.
  header: Authorization
  how_to_obtain: Run `mr-data login` to perform a device flow; the credential is stored locally at ~/.mostlyright/credentials.
  location: header
  name: device credential
  type: http-bearer
- evidence: Exactly one connector parameter named `credential_scheme`, valued `bearer` or `x-api-key`. The worker does not infer a scheme from the URL.
  how_to_obtain: Store the credential with `mr-data keys set <NAME> --value-file <FILE>` and reference it in a recipe via `secret_name`.
  location: header or query
  name: source API key / bearer token
  type: apiKey
slug: mostlyright-md-authentication
source_filename: mostlyright-md-authentication.yml
source_heading: Authentication Profile
source_url: https://mostlyright.md/docs/build/credentials/
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mostlyright.md/docs/build/credentials/\nsources:\n- https://mostlyright.md/docs/build/credentials/\n- https://mostlyright.md/docs/reference/cli/auth/\n- https://mostlyright.md/docs/build/credentials.md\n- https://mostlyright.md/docs/guides/mcp/\ndescription: Authentication methods described for Mostly Right\nschemes:\n- type: http-bearer\n  name: device credential\n  evidence: mr-data login signs this machine in to the Mostly Right cloud. It prints a short code and an approval address on stderr and opens\n    a browser. On approval it stores a durable device credential at ~/.mostlyright/credentials , mode 0600.\n  location: header\n  header: Authorization\n  how_to_obtain: Run `mr-data login` to perform a device flow; the credential is stored locally at ~/.mostlyright/credentials.\n- type: apiKey\n  name: source API key / bearer token\n  evidence: Exactly one connector parameter\
  \ named `credential_scheme`, valued `bearer` or `x-api-key`. The worker does not infer a scheme from\n    the URL.\n  location: header or query\n  how_to_obtain: Store the credential with `mr-data keys set <NAME> --value-file <FILE>` and reference it in a recipe via `secret_name`.\ndocs: https://mostlyright.md/docs/build/credentials/\n"
source_yaml_url: https://artifacts.apis.io/mostlyright-md/authentication/mostlyright-md-authentication.yml
summary_line: 2 schemes
tags:
- Data
- Finance
- Artificial Intelligence
- Datasets
- Investment
---
