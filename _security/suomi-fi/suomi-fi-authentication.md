---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: suomi-fi-connection-api-openapi.yml
  format: yaml
  label: Suomi.fi Connection API
  slug: suomi-fi-connection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-connection-api-openapi.yml
- filename: suomi-fi-countries-api-openapi.yml
  format: yaml
  label: Suomi.fi Countries API
  slug: suomi-fi-countries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-countries-api-openapi.yml
- filename: suomi-fi-general-description-api-openapi.yml
  format: yaml
  label: Suomi.fi General description API
  slug: suomi-fi-general-description-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-general-description-api-openapi.yml
- filename: suomi-fi-health-check-api-openapi.yml
  format: yaml
  label: Suomi.fi Health check API
  slug: suomi-fi-health-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-health-check-api-openapi.yml
- filename: suomi-fi-industrial-classes-api-openapi.yml
  format: yaml
  label: Suomi.fi Industrial classes API
  slug: suomi-fi-industrial-classes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-industrial-classes-api-openapi.yml
- filename: suomi-fi-languages-api-openapi.yml
  format: yaml
  label: Suomi.fi Languages API
  slug: suomi-fi-languages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-languages-api-openapi.yml
- filename: suomi-fi-life-events-api-openapi.yml
  format: yaml
  label: Suomi.fi Life events API
  slug: suomi-fi-life-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-life-events-api-openapi.yml
- filename: suomi-fi-municipalities-api-openapi.yml
  format: yaml
  label: Suomi.fi Municipalities API
  slug: suomi-fi-municipalities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-municipalities-api-openapi.yml
- filename: suomi-fi-ontology-terms-api-openapi.yml
  format: yaml
  label: Suomi.fi Ontology terms API
  slug: suomi-fi-ontology-terms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-ontology-terms-api-openapi.yml
- filename: suomi-fi-organization-api-openapi.yml
  format: yaml
  label: Suomi.fi Organization API
  slug: suomi-fi-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-organization-api-openapi.yml
- filename: suomi-fi-postal-codes-api-openapi.yml
  format: yaml
  label: Suomi.fi Postal codes API
  slug: suomi-fi-postal-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-postal-codes-api-openapi.yml
- filename: suomi-fi-regions-api-openapi.yml
  format: yaml
  label: Suomi.fi Regions API
  slug: suomi-fi-regions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-regions-api-openapi.yml
- filename: suomi-fi-service-api-openapi.yml
  format: yaml
  label: Suomi.fi Service API
  slug: suomi-fi-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-service-api-openapi.yml
- filename: suomi-fi-service-channel-api-openapi.yml
  format: yaml
  label: Suomi.fi Service channel API
  slug: suomi-fi-service-channel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-service-channel-api-openapi.yml
- filename: suomi-fi-service-classes-api-openapi.yml
  format: yaml
  label: Suomi.fi Service classes API
  slug: suomi-fi-service-classes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-service-classes-api-openapi.yml
- filename: suomi-fi-service-collection-api-openapi.yml
  format: yaml
  label: Suomi.fi Service collection API
  slug: suomi-fi-service-collection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-service-collection-api-openapi.yml
- filename: suomi-fi-target-groups-api-openapi.yml
  format: yaml
  label: Suomi.fi Target groups API
  slug: suomi-fi-target-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-target-groups-api-openapi.yml
- filename: suomi-fi-wellbeing-services-counties-api-openapi.yml
  format: yaml
  label: Suomi.fi Wellbeing services counties API
  slug: suomi-fi-wellbeing-services-counties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suomi-fi/openapi/suomi-fi-wellbeing-services-counties-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Suomi.fi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Suomi.fi secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Suomi.fi
provider_slug: suomi-fi
scheme_count: 2
schemes:
- applies_to: 30 of 32 operations (every /api/v12 read; not the two /health probes)
  description: API-key auth
  in: header
  name: apiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/_original/suomi-fi-ptv-v12-openapi.json
  type: apiKey
- applies_to: none - declared in components.securitySchemes, referenced by no operation and no root security
  bearerFormat: JWT
  description: Bearer auth
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/_original/suomi-fi-ptv-v12-openapi.json
  type: http
slug: suomi-fi-authentication
source_filename: suomi-fi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/_original/suomi-fi-ptv-v12-openapi.json\ndocs: https://kehittajille.suomi.fi/palvelut/palvelutietovaranto/rajapinta-ja-arkkitehtuuriuudistus/api-avaimen-kayttoohje-ptv-rajapintaversio-12\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  required: true\n  note: >-\n    PTV API v12 requires an API key (x-api-key header) on every read. The v12 contract applies\n    apiKeyHeader to 30 of its 32 GET operations; the two it leaves unsecured (/health/liveness,\n    /health/readiness) also answered 403 \"Invalid or missing api key\" from the production gateway\n    without a key. The contract also declares an http bearer (JWT) scheme, but no operation uses it,\n    so it is not an access requirement. The provider's own pages agree: from API version 12 an API key\n    is needed for both the search (OUT) and import (IN) APIs, issued by self-service.\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter:\
  \ x-api-key\n  description: API-key auth\n  applies_to: 30 of 32 operations (every /api/v12 read; not the two /health probes)\n  sources:\n  - openapi/_original/suomi-fi-ptv-v12-openapi.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer auth\n  applies_to: none - declared in components.securitySchemes, referenced by no operation and no root security\n  sources:\n  - openapi/_original/suomi-fi-ptv-v12-openapi.json\nversion_note: >-\n  \"The OUT interface needs no login\" is true of PTV API version 11, not version 12. The v11 contract\n  (https://api.palvelutietovaranto.suomi.fi/swagger/v11/swagger.json, title \"PTV Open Api version 11\")\n  leaves 46 of its 55 GETs unsecured and secures writes with OAuth2 implicit via palveluhallinta.suomi.fi;\n  an anonymous GET of /api/v11/CodeList/GetLanguageCodes returned 200 JSON. The production Swagger UI at\n  https://api.palvelutietovaranto.suomi.fi/swagger/ui/index.html loads that v11 document,\
  \ not a petstore\n  sample and not v12. The provider states v11 is supported until April 2027 (date to be specified).\nx-evidence:\n  fetched: '2026-11-11'\n  probes:\n  - {url: 'https://docs.palvelutietovaranto.suomi.fi/api-documentation/v12/openapi.json', status: 200, content_type: application/json, note: 'identical to openapi/_original/suomi-fi-ptv-v12-openapi.json'}\n  - {url: 'https://api-gw.palvelutietovaranto.suomi.fi/api/v12/languages', status: 403, note: 'no key: \"Invalid or missing api key\"'}\n  - {url: 'https://api-gw.palvelutietovaranto.suomi.fi/health/liveness', status: 403, note: 'no key: \"Invalid or missing api key\", although the contract declares no security here'}\n  - {url: 'https://api.palvelutietovaranto.suomi.fi/swagger/ui/index.js', status: 200, note: 'configObject.urls = /swagger/v11/swagger.json (\"Version 11\")'}\n  - {url: 'https://api.palvelutietovaranto.suomi.fi/api/v11/CodeList/GetLanguageCodes', status: 200, note: 'anonymous v11 read'}\n  - {url: 'https://kehittajille.suomi.fi/services/servicecatalogue/utilisation-of-fsc-data-and-integrations/technical-documentation-for-the-implementer-of-the-integration-api-version-12',\
  \ status: 200, note: '\"Starting in API version 12, you will need an API key for using both the search and import APIs.\"'}\n"
source_yaml_url: https://artifacts.apis.io/suomi-fi/authentication/suomi-fi-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Government
- Finland
- Public Sector
- Digital Identity
- Service Catalogue
- Open Data
- X-Road
---
