---
api_key_in: []
api_specs:
- filename: openapi-generator-clients-api-openapi.yml
  format: yaml
  label: OpenAPI Generator Clients API
  slug: openapi-generator-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openapi-generator/refs/heads/main/openapi/openapi-generator-clients-api-openapi.yml
- filename: openapi-generator-servers-api-openapi.yml
  format: yaml
  label: OpenAPI Generator Servers API
  slug: openapi-generator-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openapi-generator/refs/heads/main/openapi/openapi-generator-servers-api-openapi.yml
auth_types: []
description: 'Authentication profile for the hosted OpenAPI Generator Online API. The result is an honest zero: the service is anonymous and open. derive-authentication.py produced no profile because the Swagger 2.0 document declares no securityDefinitions block at all, and a live unauthenticated GET returned 200, confirming that this is genuinely an open API rather than a spec that merely omits its scheme.'
kind: authentication
layout: security
method: derived
name: Openapi Generator Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenAPI Generator declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: OpenAPI Generator
provider_slug: openapi-generator
scheme_count: 0
schemes: []
slug: openapi-generator-authentication
source_filename: openapi-generator-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: derived\nsource: openapi/openapi-generator-online-swagger.json + live probe of https://api.openapi-generator.tech/api/gen/clients\ndescription: >-\n  Authentication profile for the hosted OpenAPI Generator Online API. The result\n  is an honest zero: the service is anonymous and open. derive-authentication.py\n  produced no profile because the Swagger 2.0 document declares no\n  securityDefinitions block at all, and a live unauthenticated GET returned 200,\n  confirming that this is genuinely an open API rather than a spec that merely\n  omits its scheme.\nsurface: https://api.openapi-generator.tech\nspec: openapi/openapi-generator-online-swagger.json\nschemes: []\nscheme_count: 0\ndefault_security: none\nrequires_authentication: false\nevidence:\n  - {check: securityDefinitions in spec, result: absent}\n  - {check: top-level security requirement in spec, result: absent}\n  - {check: per-operation security requirement, result: absent on all\
  \ 7 operations}\n  - {url: 'https://api.openapi-generator.tech/api/gen/clients', method: GET, credentials: none, http_status: 200, fetched: '2026-08-06'}\ndeclared_error_codes_note: >-\n  Every operation declares 401 Unauthorized and 403 Forbidden. These are Spring\n  Boot framework defaults enumerated by the springfox/springdoc generator, not\n  evidence of an auth layer — no scheme exists to produce them.\ninbound_credentials_note: >-\n  The GeneratorInput request body carries an optional `authorizationValue`\n  object (keyName / type / value / urlMatcher). That credential is not for\n  authenticating to this API — it is passed THROUGH so the generator can fetch a\n  protected `openAPIUrl` on the caller's behalf. Callers should treat this as\n  sending a third-party secret to a public unauthenticated service over the open\n  internet, and prefer the CLI (cli/openapi-generator-cli.yml) for any spec that\n  requires credentials to retrieve.\noauth_scopes: none\ndocs: https://openapi-generator.tech/docs/online\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openapi-generator/refs/heads/main/authentication/openapi-generator-authentication.yml
summary_line: 0 schemes
tags:
- Code Generation
- Documentation
- Open Source
- OpenAPI
- SDK
- API Tooling
- Developer Tools
- Swagger
- Server Stubs
- Codegen
---
