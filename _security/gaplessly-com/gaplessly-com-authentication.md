---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gaplessly-com-agent-mcp-api-openapi.yml
  format: yaml
  label: Gaplessly Agent (MCP) API
  slug: gaplessly-com-agent-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gaplessly-com/openapi/gaplessly-com-agent-mcp-api-openapi.yml
- filename: gaplessly-com-appointments-engine-api-openapi.yml
  format: yaml
  label: Gaplessly Appointments engine API
  slug: gaplessly-com-appointments-engine-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gaplessly-com/openapi/gaplessly-com-appointments-engine-api-openapi.yml
- filename: gaplessly-com-guest-self-service-api-openapi.yml
  format: yaml
  label: Gaplessly Guest self-service API
  slug: gaplessly-com-guest-self-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gaplessly-com/openapi/gaplessly-com-guest-self-service-api-openapi.yml
- filename: gaplessly-com-hospitality-engine-api-openapi.yml
  format: yaml
  label: Gaplessly Hospitality engine API
  slug: gaplessly-com-hospitality-engine-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gaplessly-com/openapi/gaplessly-com-hospitality-engine-api-openapi.yml
- filename: gaplessly-com-public-booking-appointments-api-openapi.yml
  format: yaml
  label: Gaplessly Public booking (appointments) API
  slug: gaplessly-com-public-booking-appointments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gaplessly-com/openapi/gaplessly-com-public-booking-appointments-api-openapi.yml
- filename: gaplessly-com-public-booking-hospitality-api-openapi.yml
  format: yaml
  label: Gaplessly Public booking (hospitality) API
  slug: gaplessly-com-public-booking-hospitality-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gaplessly-com/openapi/gaplessly-com-public-booking-hospitality-api-openapi.yml
- filename: gaplessly-com-shared-api-openapi.yml
  format: yaml
  label: Gaplessly Shared API
  slug: gaplessly-com-shared-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gaplessly-com/openapi/gaplessly-com-shared-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Gaplessly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gaplessly declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Gaplessly
provider_slug: gaplessly-com
scheme_count: 1
schemes:
- evidence: 'Send it as Authorization: Bearer sk_live_… and nowhere else: no query parameter, custom header or cookie, because a credential in a URL ends up in logs and browser history.'
  header: Authorization
  how_to_obtain: An organization admin creates keys in the dashboard under Developer; the raw key is shown once when it is created.
  location: header
  name: Bearer
  scopes:
  - clients:read
  - clients:write
  - organization:read
  - availability:read
  - webhooks:write
  - services:read
  - services:write
  - providers:read
  - providers:write
  - appointments:read
  - appointments:write
  - tables:read
  - tables:write
  - service-periods:read
  - service-periods:write
  - reservations:read
  - reservations:write
  type: http-bearer
slug: gaplessly-com-authentication
source_filename: gaplessly-com-authentication.yml
source_heading: Authentication Profile
source_url: https://gaplessly.com/.well-known/oauth-protected-resource
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://gaplessly.com/.well-known/oauth-protected-resource\nsources:\n- https://gaplessly.com/.well-known/oauth-protected-resource\n- https://gaplessly.com/docs/authentication\n- https://gaplessly.com/docs/reference/hospitality-engine/setReservationStatusV1\n- https://gaplessly.com/docs/reference/hospitality-engine/moveReservationTableV1\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send it as Authorization: Bearer sk_live_… and nowhere else: no query parameter, custom header or cookie, because a credential in\n    a URL ends up in logs and browser history.'\n  location: header\n  header: Authorization\n  scopes:\n  - clients:read\n  - clients:write\n  - organization:read\n  - availability:read\n  - webhooks:write\n  - services:read\n  - services:write\n  - providers:read\n  - providers:write\n  - appointments:read\n  - appointments:write\n  - tables:read\n  - tables:write\n\
  \  - service-periods:read\n  - service-periods:write\n  - reservations:read\n  - reservations:write\n  how_to_obtain: An organization admin creates keys in the dashboard under Developer; the raw key is shown once when it is created.\nnote: No OAuth2 flows are documented on the provided pages.\ndocs: https://gaplessly.com/.well-known/oauth-protected-resource\n"
source_yaml_url: https://artifacts.apis.io/gaplessly-com/authentication/gaplessly-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Booking
- Software-as-a-Service
- Restaurant
- Scheduling
---
