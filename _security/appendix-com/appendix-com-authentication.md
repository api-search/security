---
anonymous_access: false
api_key_in: []
api_specs:
- filename: appendix-com-api-reference-openapi-generated.yml
  format: yaml
  label: Appendix api reference API
  slug: api-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appendix-com/openapi/_ae-authored/appendix-com-api-reference-openapi-generated.yml
- filename: appendix-com-core-openapi-generated.yml
  format: yaml
  label: Appendix core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appendix-com/openapi/_ae-authored/appendix-com-core-openapi-generated.yml
- filename: appendix-com-prescribing-openapi-generated.yml
  format: yaml
  label: Appendix Prescribing API Overview API
  slug: prescribing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appendix-com/openapi/_ae-authored/appendix-com-prescribing-openapi-generated.yml
auth_types: []
description: Authentication schemes as described on the Appendix documentation pages.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Appendix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Appendix declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Appendix
provider_slug: appendix-com
scheme_count: 3
schemes:
- evidence: 'Send it as Authorization: Bearer ak_… (or X-API-Key ) on any authenticated endpoint except account and credential management'
  header: Authorization
  how_to_obtain: Mint a personal API key (ak_…) from your account dashboard after creating an Appendix account.
  location: header
  name: Personal API Key
  type: apiKey
- evidence: 'Send it as Authorization: Bearer ak_… (or X-API-Key ) on any authenticated endpoint except account and credential management'
  header: X-API-Key
  how_to_obtain: Mint a personal API key (ak_…) from your account dashboard after creating an Appendix account.
  location: header
  name: Personal API Key (alternative header)
  type: apiKey
- evidence: The first request your agent makes — POST /api/v1/agent/query — is fully public. There is no API key, no OAuth, no signed token to obtain.
  name: Anonymous (no credentials)
  type: other
slug: appendix-com-authentication
source_filename: appendix-com-authentication.yml
source_heading: Authentication Profile
source_url: https://appendix.com/docs/api-reference/authentication
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://appendix.com/docs/api-reference/authentication\nsources:\n- https://appendix.com/docs/api-reference/authentication\n- https://appendix.com/docs/prescribing-api/quickstart\n- https://appendix.com/docs/api-reference/quick-start\ndescription: Authentication schemes as described on the Appendix documentation pages.\nschemes:\n- type: apiKey\n  name: Personal API Key\n  evidence: 'Send it as Authorization: Bearer ak_… (or X-API-Key ) on any authenticated endpoint except account and credential management'\n  location: header\n  header: Authorization\n  how_to_obtain: Mint a personal API key (ak_…) from your account dashboard after creating an Appendix account.\n- type: apiKey\n  name: Personal API Key (alternative header)\n  evidence: 'Send it as Authorization: Bearer ak_… (or X-API-Key ) on any authenticated endpoint except account and credential management'\n  location: header\n\
  \  header: X-API-Key\n  how_to_obtain: Mint a personal API key (ak_…) from your account dashboard after creating an Appendix account.\n- type: other\n  name: Anonymous (no credentials)\n  evidence: The first request your agent makes — POST /api/v1/agent/query — is fully public. There is no API key, no OAuth, no signed token to\n    obtain.\ndocs: https://appendix.com/docs/api-reference/authentication\n"
source_yaml_url: https://artifacts.apis.io/appendix-com/authentication/appendix-com-authentication.yml
summary_line: 3 schemes
tags:
- Healthcare
- Artificial Intelligence
- Telehealth
- PhysicianReview
---
