---
api_key_in: []
api_specs:
- filename: elisa-categories-api-openapi.yml
  format: yaml
  label: ELISA Categories API
  slug: elisa-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elisa/refs/heads/main/openapi/elisa-categories-api-openapi.yml
- filename: elisa-doc-api-openapi.yml
  format: yaml
  label: ELISA Doc API
  slug: elisa-doc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elisa/refs/heads/main/openapi/elisa-doc-api-openapi.yml
- filename: elisa-events-api-openapi.yml
  format: yaml
  label: ELISA Events API
  slug: elisa-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elisa/refs/heads/main/openapi/elisa-events-api-openapi.yml
- filename: elisa-organizers-api-openapi.yml
  format: yaml
  label: ELISA Organizers API
  slug: elisa-organizers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elisa/refs/heads/main/openapi/elisa-organizers-api-openapi.yml
- filename: elisa-tags-api-openapi.yml
  format: yaml
  label: ELISA Tags API
  slug: elisa-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elisa/refs/heads/main/openapi/elisa-tags-api-openapi.yml
- filename: elisa-venues-api-openapi.yml
  format: yaml
  label: ELISA Venues API
  slug: elisa-venues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elisa/refs/heads/main/openapi/elisa-venues-api-openapi.yml
auth_types: []
description: Authentication profile for the ELISA API surface at https://elisa.tech/wp-json/. Established by reading the authentication block the WordPress REST root advertises about itself and by making live unauthenticated calls against the published operations.
kind: authentication
layout: security
method: probed
name: Elisa Authentication
name_suffix: Authentication
oauth_flows: []
overview: ELISA declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ELISA
provider_slug: elisa
scheme_count: 2
schemes:
- applies_to: all GET operations
  evidence: GET https://elisa.tech/wp-json/tribe/events/v1/events?per_page=1 returned 200 with a real ELISA event payload (7,701 bytes) on an unauthenticated request, 2026-08-27.
  id: anonymous
  type: none
  verified: probed
- applies_to: all POST and DELETE operations
  authorization_endpoint: https://elisa.tech/wp-admin/authorize-application.php
  detail: A WordPress Application Password is a per-user, per-application credential presented over HTTP Basic (username plus the generated password). It is not scoped — it inherits the full capability set of the WordPress user it belongs to. There is no OAuth, no OIDC, no API-key header, and no mTLS on this surface.
  evidence: The /wp-json/ root document advertises authentication.application-passwords.endpoints.authorization = https://elisa.tech/wp-admin/authorize-application.php, and it is the only scheme it names.
  id: application-passwords
  obtain: A site administrator generates one from the user profile screen in wp-admin, or the application initiates the authorize-application.php flow. ELISA does not publish a self-service developer signup for API credentials; write access implies a WordPress account on elisa.tech.
  scheme: basic
  type: http
  verified: probed
slug: elisa-authentication
source_filename: elisa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: https://elisa.tech/wp-json/ (authentication block) + openapi/elisa-events-calendar-openapi.json\nprovider: ELISA\nproviderId: elisa\ndescription: >-\n  Authentication profile for the ELISA API surface at https://elisa.tech/wp-json/. Established by\n  reading the authentication block the WordPress REST root advertises about itself and by making\n  live unauthenticated calls against the published operations.\nsummary: >-\n  Reads are open; writes are WordPress-capability gated behind HTTP Basic with an Application\n  Password. The OpenAPI document declares no securitySchemes at all, so the auth model is carried\n  entirely by the platform rather than by the contract — a real gap for any agent that plans from\n  the spec alone.\nspec_declares_security_schemes: false\nschemes:\n  - id: anonymous\n    type: none\n    applies_to: all GET operations\n    verified: probed\n    evidence: >-\n      GET https://elisa.tech/wp-json/tribe/events/v1/events?per_page=1\
  \ returned 200 with a real\n      ELISA event payload (7,701 bytes) on an unauthenticated request, 2026-08-27.\n  - id: application-passwords\n    type: http\n    scheme: basic\n    applies_to: all POST and DELETE operations\n    verified: probed\n    authorization_endpoint: https://elisa.tech/wp-admin/authorize-application.php\n    evidence: >-\n      The /wp-json/ root document advertises\n      authentication.application-passwords.endpoints.authorization =\n      https://elisa.tech/wp-admin/authorize-application.php, and it is the only scheme it names.\n    detail: >-\n      A WordPress Application Password is a per-user, per-application credential presented over\n      HTTP Basic (username plus the generated password). It is not scoped — it inherits the full\n      capability set of the WordPress user it belongs to. There is no OAuth, no OIDC, no API-key\n      header, and no mTLS on this surface.\n    obtain: >-\n      A site administrator generates one from the user profile screen\
  \ in wp-admin, or the\n      application initiates the authorize-application.php flow. ELISA does not publish a\n      self-service developer signup for API credentials; write access implies a WordPress account\n      on elisa.tech.\nauthorization_model:\n  style: wordpress-capabilities\n  scopes: none\n  note: >-\n    Permission is decided by WordPress capabilities (edit_posts, delete_posts and the Events\n    Calendar equivalents), not by scopes. This is why scopes/ is deliberately absent for this\n    provider rather than empty — there is no scope surface to document.\nobserved_denials:\n  - operation: GET /wp-json/wp-abilities/v1/abilities\n    status: 401\n    body: '{\"code\":\"rest_forbidden\",\"message\":\"Sorry, you are not allowed to do that.\",\"data\":{\"status\":401}}'\n    note: >-\n      The WordPress Abilities API namespace (wp-abilities/v1) is registered on this site — it is an\n      agent-facing capability registry — but its abilities listing is authenticated. The namespace\n\
  \      index at /wp-json/wp-abilities/v1 is readable anonymously; the abilities themselves are not.\ngaps:\n  - The OpenAPI declares no securitySchemes and applies no security to any operation, so a client generated from the spec has no way to know that POST and DELETE need credentials.\n  - No published developer-credential path — obtaining write access requires an ELISA WordPress account, which is not a self-service developer program.\ncross_references:\n  conventions: conventions/elisa-conventions.yml\n  well_known: well-known/elisa-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elisa/refs/heads/main/authentication/elisa-authentication.yml
summary_line: 2 schemes
tags:
- Embedded
- Linux
- Linux Foundation
- Safety
- Functional Safety
- Open-Source
- Automotive
- Aerospace
- Medical Devices
- Traceability
- Standards
- Event
---
