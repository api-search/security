---
anonymous_access: false
api_key_in: []
api_specs:
- filename: regfish-com-openapi-generated.yml
  format: yaml
  label: regfish API
  slug: regfish-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/regfish-com/openapi/_ae-authored/regfish-com-openapi-generated.yml
auth_types: []
description: Authentication schemes for regfish API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: regfish Authentication
name_suffix: Authentication
oauth_flows: []
overview: regfish declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: regfish
provider_slug: regfish-com
scheme_count: 1
schemes:
- evidence: Jeder Aufruf der regfish-API braucht einen API-Key im Header x-api-key.
  header: x-api-key
  how_to_obtain: Erstellt im dash unter Konto → Sicherheit → API Keys
  location: header
  name: API Key
  type: apiKey
slug: regfish-com-authentication
source_filename: regfish-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.regfish.com/de/dash/api-keys/
source_yaml: "generated: '2026-11-23'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.regfish.com/de/dash/api-keys/\nsources:\n- https://docs.regfish.com/de/dash/api-keys/\n- https://docs.regfish.com/de/reference/meta/get-token-info/\n- https://docs.regfish.com/de/getting-started/\n- https://docs.regfish.com/de/recipes/dyndns-fritzbox-setup/\ndescription: Authentication schemes for regfish API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Jeder Aufruf der regfish-API braucht einen API-Key im Header x-api-key.\n  location: header\n  header: x-api-key\n  how_to_obtain: Erstellt im dash unter Konto → Sicherheit → API Keys\ndocs: https://docs.regfish.com/de/dash/api-keys/\n"
source_yaml_url: https://artifacts.apis.io/regfish-com/authentication/regfish-com-authentication.yml
summary_line: 1 scheme
tags:
- Domains
- Email Hosting
- Web Hosting
- DNS
- API
- Managed WordPress
- Agency Plans
---
