---
anonymous_access: false
api_key_in: []
api_specs:
- filename: enterprise-wikimedia-com-articles-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Articles API
  slug: enterprise-wikimedia-com-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-articles-api-openapi.yml
- filename: enterprise-wikimedia-com-authentication-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Authentication API
  slug: enterprise-wikimedia-com-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-authentication-api-openapi.yml
- filename: enterprise-wikimedia-com-batches-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Batches API
  slug: enterprise-wikimedia-com-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-batches-api-openapi.yml
- filename: enterprise-wikimedia-com-codes-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Codes API
  slug: enterprise-wikimedia-com-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-codes-api-openapi.yml
- filename: enterprise-wikimedia-com-languages-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Languages API
  slug: enterprise-wikimedia-com-languages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-languages-api-openapi.yml
- filename: enterprise-wikimedia-com-namespaces-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Namespaces API
  slug: enterprise-wikimedia-com-namespaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-namespaces-api-openapi.yml
- filename: enterprise-wikimedia-com-projects-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Projects API
  slug: enterprise-wikimedia-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-projects-api-openapi.yml
- filename: enterprise-wikimedia-com-realtime-articles-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Realtime Articles API
  slug: enterprise-wikimedia-com-realtime-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-realtime-articles-api-openapi.yml
- filename: enterprise-wikimedia-com-realtime-wikidata-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Realtime Wikidata API
  slug: enterprise-wikimedia-com-realtime-wikidata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-realtime-wikidata-api-openapi.yml
- filename: enterprise-wikimedia-com-snapshots-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Snapshots API
  slug: enterprise-wikimedia-com-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-snapshots-api-openapi.yml
- filename: enterprise-wikimedia-com-structured-contents-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Structured Contents API
  slug: enterprise-wikimedia-com-structured-contents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-structured-contents-api-openapi.yml
- filename: enterprise-wikimedia-com-structured-snapshots-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Structured Snapshots API
  slug: enterprise-wikimedia-com-structured-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-structured-snapshots-api-openapi.yml
- filename: enterprise-wikimedia-com-wikidata-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Wikidata API
  slug: enterprise-wikimedia-com-wikidata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-wikidata-api-openapi.yml
- filename: enterprise-wikimedia-com-wikidata-batches-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Wikidata Batches API
  slug: enterprise-wikimedia-com-wikidata-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-wikidata-batches-api-openapi.yml
- filename: enterprise-wikimedia-com-wikidata-snapshots-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Wikidata Snapshots API
  slug: enterprise-wikimedia-com-wikidata-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-wikidata-snapshots-api-openapi.yml
auth_types: []
description: 'Wikimedia Enterprise APIs use JWT authentication passed in the header: all requests must be made over HTTPS and pass a Bearer access token in the `Authorization` header.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Wikimedia Enterprise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wikimedia Enterprise declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Wikimedia Enterprise
provider_slug: enterprise-wikimedia-com
scheme_count: 1
schemes:
- evidence: 'Wikimedia Enterprise APIs use JWT authentication passed in the header: all requests must be made over HTTPS and pass a Bearer access token in the `Authorization` header.'
  header: Authorization
  how_to_obtain: Use the Login endpoint to receive an access token, then include it as a Bearer token in the Authorization header of each request.
  location: header
  name: Bearer
  type: http-bearer
slug: enterprise-wikimedia-com-authentication
source_filename: enterprise-wikimedia-com-authentication.yml
source_heading: Authentication Profile
source_url: https://enterprise.wikimedia.com/docs/authentication.md
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://enterprise.wikimedia.com/docs/authentication.md\nsources:\n- https://enterprise.wikimedia.com/docs/authentication.md\n- https://enterprise.wikimedia.com/docs/authentication/\n- https://enterprise.wikimedia.com/docs/agents.md\n- https://enterprise.wikimedia.com/docs/index.md\ndescription: 'Wikimedia Enterprise APIs use JWT authentication passed in the header: all requests must be made over HTTPS and pass a Bearer access\n  token in the `Authorization` header.'\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Wikimedia Enterprise APIs use JWT authentication passed in the header: all requests must be made over HTTPS and pass a Bearer access\n    token in the `Authorization` header.'\n  location: header\n  header: Authorization\n  how_to_obtain: Use the Login endpoint to receive an access token, then include it as a Bearer token in the Authorization header of each\
  \ request.\ndocs: https://enterprise.wikimedia.com/docs/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/enterprise-wikimedia-com/authentication/enterprise-wikimedia-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Data
- Enterprise
- Wikimedia
---
