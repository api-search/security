---
anonymous_access: false
api_key_in: []
api_specs:
- filename: domaindrift-io-alerts-api-openapi.yml
  format: yaml
  label: DomainDrift Alerts API
  slug: domaindrift-io-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domaindrift-io/openapi/domaindrift-io-alerts-api-openapi.yml
- filename: domaindrift-io-changes-api-openapi.yml
  format: yaml
  label: DomainDrift Changes API
  slug: domaindrift-io-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domaindrift-io/openapi/domaindrift-io-changes-api-openapi.yml
- filename: domaindrift-io-domains-api-openapi.yml
  format: yaml
  label: DomainDrift Domains API
  slug: domaindrift-io-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domaindrift-io/openapi/domaindrift-io-domains-api-openapi.yml
- filename: domaindrift-io-health-api-openapi.yml
  format: yaml
  label: DomainDrift Health API
  slug: domaindrift-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domaindrift-io/openapi/domaindrift-io-health-api-openapi.yml
- filename: domaindrift-io-scan-api-openapi.yml
  format: yaml
  label: DomainDrift Scan API
  slug: domaindrift-io-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domaindrift-io/openapi/domaindrift-io-scan-api-openapi.yml
- filename: domaindrift-io-stream-api-openapi.yml
  format: yaml
  label: DomainDrift Stream API
  slug: domaindrift-io-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domaindrift-io/openapi/domaindrift-io-stream-api-openapi.yml
auth_types: []
description: Authentication methods for DomainDrift API as documented on the Getting Started page.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Domaindrift Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: DomainDrift declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: DomainDrift
provider_slug: domaindrift-io
scheme_count: 2
schemes:
- evidence: 'curl -H "X-DomainDrift-Key: dd_..." https://domaindrift.io/v1/domains/example.com'
  header: X-DomainDrift-Key
  how_to_obtain: Mint your API key from the API console.
  location: header
  name: X-DomainDrift-Key
  type: apiKey
- evidence: 'curl -H "Authorization: Bearer dd_..." https://domaindrift.io/v1/domains/example.com'
  header: Authorization
  how_to_obtain: Mint your API key from the API console.
  location: header
  name: Authorization
  type: http-bearer
slug: domaindrift-io-authentication
source_filename: domaindrift-io-authentication.yml
source_heading: Authentication Profile
source_url: https://domaindrift.io/docs/getting-started
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://domaindrift.io/docs/getting-started\nsources:\n- https://domaindrift.io/docs/getting-started\ndescription: Authentication methods for DomainDrift API as documented on the Getting Started page.\nschemes:\n- type: apiKey\n  name: X-DomainDrift-Key\n  evidence: 'curl -H \"X-DomainDrift-Key: dd_...\" https://domaindrift.io/v1/domains/example.com'\n  location: header\n  header: X-DomainDrift-Key\n  how_to_obtain: Mint your API key from the API console.\n- type: http-bearer\n  name: Authorization\n  evidence: 'curl -H \"Authorization: Bearer dd_...\" https://domaindrift.io/v1/domains/example.com'\n  location: header\n  header: Authorization\n  how_to_obtain: Mint your API key from the API console.\nnote: No OAuth2, http-basic, jwt, hmac, mtls, or other authentication schemes are mentioned on the page.\ndocs: https://domaindrift.io/docs/getting-started\n"
source_yaml_url: https://artifacts.apis.io/domaindrift-io/authentication/domaindrift-io-authentication.yml
summary_line: 2 schemes
tags:
- Security
- Monitoring
- Domain
- Telemetry
---
