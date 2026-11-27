---
anonymous_access: false
api_key_in: []
api_specs:
- filename: jennipro-com-account-api-openapi.yml
  format: yaml
  label: JENNi Account API
  slug: jennipro-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jennipro-com/openapi/jennipro-com-account-api-openapi.yml
- filename: jennipro-com-brand-portal-api-openapi.yml
  format: yaml
  label: JENNi Brand portal API
  slug: jennipro-com-brand-portal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jennipro-com/openapi/jennipro-com-brand-portal-api-openapi.yml
- filename: jennipro-com-catalog-api-openapi.yml
  format: yaml
  label: JENNi Catalog API
  slug: jennipro-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jennipro-com/openapi/jennipro-com-catalog-api-openapi.yml
- filename: jennipro-com-channel-api-openapi.yml
  format: yaml
  label: JENNi Channel API
  slug: jennipro-com-channel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jennipro-com/openapi/jennipro-com-channel-api-openapi.yml
- filename: jennipro-com-events-api-openapi.yml
  format: yaml
  label: JENNi Events API
  slug: jennipro-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jennipro-com/openapi/jennipro-com-events-api-openapi.yml
- filename: jennipro-com-inventory-api-openapi.yml
  format: yaml
  label: JENNi Inventory API
  slug: jennipro-com-inventory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jennipro-com/openapi/jennipro-com-inventory-api-openapi.yml
- filename: jennipro-com-portal-api-openapi.yml
  format: yaml
  label: JENNi Portal API
  slug: jennipro-com-portal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jennipro-com/openapi/jennipro-com-portal-api-openapi.yml
- filename: jennipro-com-retailers-api-openapi.yml
  format: yaml
  label: JENNi Retailers API
  slug: jennipro-com-retailers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jennipro-com/openapi/jennipro-com-retailers-api-openapi.yml
- filename: jennipro-com-runs-api-openapi.yml
  format: yaml
  label: JENNi Runs API
  slug: jennipro-com-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jennipro-com/openapi/jennipro-com-runs-api-openapi.yml
- filename: jennipro-com-service-api-openapi.yml
  format: yaml
  label: JENNi Service API
  slug: jennipro-com-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jennipro-com/openapi/jennipro-com-service-api-openapi.yml
- filename: jennipro-com-stores-api-openapi.yml
  format: yaml
  label: JENNi Stores API
  slug: jennipro-com-stores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jennipro-com/openapi/jennipro-com-stores-api-openapi.yml
- filename: jennipro-com-webhooks-api-openapi.yml
  format: yaml
  label: JENNi Webhooks API
  slug: jennipro-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jennipro-com/openapi/jennipro-com-webhooks-api-openapi.yml
auth_types: []
description: Partner API key authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: JENNi Authentication
name_suffix: Authentication
oauth_flows: []
overview: JENNi declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: JENNi
provider_slug: jennipro-com
scheme_count: 1
schemes:
- evidence: 'Every authenticated request to /provider/v1/* or /channel/v1/* carries one header: X-Jenni-Api-Key: {keyId}.{secret}'
  header: X-Jenni-Api-Key
  how_to_obtain: Request a key via the JENNi portal (Sign in / Sign up → Keys tab → Request a key). The secret is shown once and must be used as <keyId>.<secret>.
  location: header
  name: PartnerApiKey
  type: apiKey
slug: jennipro-com-authentication
source_filename: jennipro-com-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.jennipro.com/#tag/authentication
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.jennipro.com/#tag/authentication\nsources:\n- https://developer.jennipro.com/#tag/authentication\n- https://developer.jennipro.com/#tag/quickstart\ndescription: Partner API key authentication\nschemes:\n- type: apiKey\n  name: PartnerApiKey\n  evidence: 'Every authenticated request to /provider/v1/* or /channel/v1/* carries one header: X-Jenni-Api-Key: {keyId}.{secret}'\n  location: header\n  header: X-Jenni-Api-Key\n  how_to_obtain: Request a key via the JENNi portal (Sign in / Sign up → Keys tab → Request a key). The secret is shown once and must be used\n    as <keyId>.<secret>.\nnote: No OAuth2, bearer, or other authentication methods are documented.\ndocs: https://developer.jennipro.com/#tag/authentication\n"
source_yaml_url: https://artifacts.apis.io/jennipro-com/authentication/jennipro-com-authentication.yml
summary_line: 1 scheme
tags:
- Inventory
- Retail
- Supply Chain
- Marketplace
---
