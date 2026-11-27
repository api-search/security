---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dnsmint-com-api-openapi.json
  format: json
  label: DNSMint API API
  slug: dnsmint-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dnsmint-com/openapi/_original/dnsmint-com-api-openapi.json
auth_types: []
description: Authentication uses an API key provided as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: DNSMint Authentication
name_suffix: Authentication
oauth_flows: []
overview: DNSMint declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DNSMint
provider_slug: dnsmint-com
scheme_count: 1
schemes:
- evidence: '-H "Authorization: Bearer $DNSMINT_KEY"'
  header: Authorization
  how_to_obtain: Create an API key in the dashboard after signing in; the key looks like dnsm_<key_id>_<secret>.
  location: header
  name: Bearer
  type: http-bearer
slug: dnsmint-com-authentication
source_filename: dnsmint-com-authentication.yml
source_heading: Authentication Profile
source_url: https://dnsmint.com/quickstart
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dnsmint.com/quickstart\nsources:\n- https://dnsmint.com/quickstart\ndescription: Authentication uses an API key provided as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: '-H \"Authorization: Bearer $DNSMINT_KEY\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the dashboard after signing in; the key looks like dnsm_<key_id>_<secret>.\ndocs: https://dnsmint.com/quickstart\n"
source_yaml_url: https://artifacts.apis.io/dnsmint-com/authentication/dnsmint-com-authentication.yml
summary_line: 1 scheme
tags:
- DNS
- Automation
- Infrastructure
- Cloud
---
