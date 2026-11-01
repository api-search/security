---
anonymous_access: false
api_key_in: []
api_specs:
- filename: allratestoday-com-authentication-api-openapi.yml
  format: yaml
  label: allratestoday-com Authentication API
  slug: allratestoday-com-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allratestoday-com/openapi/allratestoday-com-authentication-api-openapi.yml
- filename: allratestoday-com-central-bank-rates-api-openapi.yml
  format: yaml
  label: allratestoday-com Central Bank Rates API
  slug: allratestoday-com-central-bank-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allratestoday-com/openapi/allratestoday-com-central-bank-rates-api-openapi.yml
- filename: allratestoday-com-compatibility-api-openapi.yml
  format: yaml
  label: allratestoday-com Compatibility API
  slug: allratestoday-com-compatibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allratestoday-com/openapi/allratestoday-com-compatibility-api-openapi.yml
- filename: allratestoday-com-market-rates-api-openapi.yml
  format: yaml
  label: allratestoday-com Market Rates API
  slug: allratestoday-com-market-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allratestoday-com/openapi/allratestoday-com-market-rates-api-openapi.yml
- filename: allratestoday-com-open-endpoints-api-openapi.yml
  format: yaml
  label: allratestoday-com Open Endpoints API
  slug: allratestoday-com-open-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allratestoday-com/openapi/allratestoday-com-open-endpoints-api-openapi.yml
- filename: allratestoday-com-reference-rate-api-openapi.yml
  format: yaml
  label: allratestoday-com Reference Rate API
  slug: allratestoday-com-reference-rate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allratestoday-com/openapi/allratestoday-com-reference-rate-api-openapi.yml
auth_types: []
description: Authentication is performed by sending the AllRatesToday API key as a Bearer token in the Authorization header, or alternatively as an api_key query parameter.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Allratestoday Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: allratestoday-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: allratestoday-com
provider_slug: allratestoday-com
scheme_count: 2
schemes:
- evidence: 'To use your key, send it as Authorization: Bearer art_live_…'
  header: Authorization
  how_to_obtain: Sign up at allratestoday.com/register, verify email, and copy the key from your dashboard (it begins with art_live_).
  location: header
  name: Bearer
  type: http-bearer
- evidence: where the client only accepts a URL, connect to https://allratestoday.com/api/mcp?api_key=art_live_…
  how_to_obtain: Sign up at allratestoday.com/register, verify email, and copy the key from your dashboard (it begins with art_live_).
  location: query
  name: api_key query
  type: apiKey
slug: allratestoday-com-authentication
source_filename: allratestoday-com-authentication.yml
source_heading: Authentication Profile
source_url: https://allratestoday.com/docs/mcp-server/
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://allratestoday.com/docs/mcp-server/\nsources:\n- https://allratestoday.com/docs/mcp-server/\n- https://allratestoday.com/docs/mcp-server\ndescription: Authentication is performed by sending the AllRatesToday API key as a Bearer token in the Authorization header, or alternatively\n  as an api_key query parameter.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'To use your key, send it as Authorization: Bearer art_live_…'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign up at allratestoday.com/register, verify email, and copy the key from your dashboard (it begins with art_live_).\n- type: apiKey\n  name: api_key query\n  evidence: where the client only accepts a URL, connect to https://allratestoday.com/api/mcp?api_key=art_live_…\n  location: query\n  how_to_obtain: Sign up at allratestoday.com/register, verify email, and copy the key from your\
  \ dashboard (it begins with art_live_).\nnote: No OAuth2 flows are described on the pages.\ndocs: https://allratestoday.com/docs/mcp-server/\n"
source_yaml_url: https://artifacts.apis.io/allratestoday-com/authentication/allratestoday-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Fintech
- ExchangeRates
- API
- Data
---
