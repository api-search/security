---
anonymous_access: false
api_key_in: []
api_specs:
- filename: favcrm-io-content-api-openapi.yml
  format: yaml
  label: FavCRM Content API
  slug: favcrm-io-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/favcrm-io/openapi/favcrm-io-content-api-openapi.yml
- filename: favcrm-io-events-api-openapi.yml
  format: yaml
  label: FavCRM Events API
  slug: favcrm-io-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/favcrm-io/openapi/favcrm-io-events-api-openapi.yml
- filename: favcrm-io-forms-and-surveys-api-openapi.yml
  format: yaml
  label: FavCRM Forms and Surveys API
  slug: favcrm-io-forms-and-surveys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/favcrm-io/openapi/favcrm-io-forms-and-surveys-api-openapi.yml
- filename: favcrm-io-loyalty-and-offers-api-openapi.yml
  format: yaml
  label: FavCRM Loyalty and Offers API
  slug: favcrm-io-loyalty-and-offers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/favcrm-io/openapi/favcrm-io-loyalty-and-offers-api-openapi.yml
- filename: favcrm-io-member-session-api-openapi.yml
  format: yaml
  label: FavCRM Member Session API
  slug: favcrm-io-member-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/favcrm-io/openapi/favcrm-io-member-session-api-openapi.yml
- filename: favcrm-io-service-booking-api-openapi.yml
  format: yaml
  label: FavCRM Service Booking API
  slug: favcrm-io-service-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/favcrm-io/openapi/favcrm-io-service-booking-api-openapi.yml
- filename: favcrm-io-shop-api-openapi.yml
  format: yaml
  label: FavCRM Shop API
  slug: favcrm-io-shop-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/favcrm-io/openapi/favcrm-io-shop-api-openapi.yml
auth_types: []
description: Authentication methods for FavCRM MCP as described on the page.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Favcrm Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: FavCRM declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: FavCRM
provider_slug: favcrm-io
scheme_count: 2
schemes:
- authorize_url: https://api.favcrm.io/mcp/oauth/manage
  evidence: OAuth sign-in (default) | `https://api.favcrm.io/mcp/oauth/manage`
  flows:
  - authorization_code
  how_to_obtain: User signs in via the provided OAuth URL, selects workspace, reviews requested scopes, and approves or denies access.
  name: OAuth sign-in (default)
  type: oauth2
- authorize_url: https://api.favcrm.io/mcp/oauth/view
  evidence: OAuth sign-in, read-only | `https://api.favcrm.io/mcp/oauth/view`
  flows:
  - authorization_code
  how_to_obtain: User signs in via the read‑only OAuth URL, selects workspace, reviews requested scopes, and approves or denies access.
  name: OAuth sign-in, read-only
  type: oauth2
slug: favcrm-io-authentication
source_filename: favcrm-io-authentication.yml
source_heading: Authentication Profile
source_url: https://favcrm.io/docs/simply-booking-mcp.md
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://favcrm.io/docs/simply-booking-mcp.md\nsources:\n- https://favcrm.io/docs/simply-booking-mcp.md\ndescription: Authentication methods for FavCRM MCP as described on the page.\nschemes:\n- type: oauth2\n  name: OAuth sign-in (default)\n  evidence: OAuth sign-in (default) | `https://api.favcrm.io/mcp/oauth/manage`\n  flows:\n  - authorization_code\n  authorize_url: https://api.favcrm.io/mcp/oauth/manage\n  how_to_obtain: User signs in via the provided OAuth URL, selects workspace, reviews requested scopes, and approves or denies access.\n- type: oauth2\n  name: OAuth sign-in, read-only\n  evidence: OAuth sign-in, read-only | `https://api.favcrm.io/mcp/oauth/view`\n  flows:\n  - authorization_code\n  authorize_url: https://api.favcrm.io/mcp/oauth/view\n  how_to_obtain: User signs in via the read‑only OAuth URL, selects workspace, reviews requested scopes, and approves or denies\
  \ access.\ndocs: https://favcrm.io/docs/simply-booking-mcp.md\n"
source_yaml_url: https://artifacts.apis.io/favcrm-io/authentication/favcrm-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- CRM
- Appointment
- Membership
- WhatsApp
- AI
---
