---
anonymous_access: false
api_key_in: []
api_specs:
- filename: astrocal-dev-activity-api-openapi.yml
  format: yaml
  label: Astrocal Activity API
  slug: astrocal-dev-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astrocal-dev/openapi/astrocal-dev-activity-api-openapi.yml
- filename: astrocal-dev-api-keys-api-openapi.yml
  format: yaml
  label: Astrocal API Keys API
  slug: astrocal-dev-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astrocal-dev/openapi/astrocal-dev-api-keys-api-openapi.yml
- filename: astrocal-dev-availability-api-openapi.yml
  format: yaml
  label: Astrocal Availability API
  slug: astrocal-dev-availability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astrocal-dev/openapi/astrocal-dev-availability-api-openapi.yml
- filename: astrocal-dev-booking-pages-api-openapi.yml
  format: yaml
  label: Astrocal Booking Pages API
  slug: astrocal-dev-booking-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astrocal-dev/openapi/astrocal-dev-booking-pages-api-openapi.yml
- filename: astrocal-dev-bookings-api-openapi.yml
  format: yaml
  label: Astrocal Bookings API
  slug: astrocal-dev-bookings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astrocal-dev/openapi/astrocal-dev-bookings-api-openapi.yml
- filename: astrocal-dev-branding-api-openapi.yml
  format: yaml
  label: Astrocal Branding API
  slug: astrocal-dev-branding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astrocal-dev/openapi/astrocal-dev-branding-api-openapi.yml
- filename: astrocal-dev-calendars-api-openapi.yml
  format: yaml
  label: Astrocal Calendars API
  slug: astrocal-dev-calendars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astrocal-dev/openapi/astrocal-dev-calendars-api-openapi.yml
- filename: astrocal-dev-conferencing-api-openapi.yml
  format: yaml
  label: Astrocal Conferencing API
  slug: astrocal-dev-conferencing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astrocal-dev/openapi/astrocal-dev-conferencing-api-openapi.yml
- filename: astrocal-dev-event-type-hosts-api-openapi.yml
  format: yaml
  label: Astrocal Event Type Hosts API
  slug: astrocal-dev-event-type-hosts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astrocal-dev/openapi/astrocal-dev-event-type-hosts-api-openapi.yml
- filename: astrocal-dev-event-types-api-openapi.yml
  format: yaml
  label: Astrocal Event Types API
  slug: astrocal-dev-event-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astrocal-dev/openapi/astrocal-dev-event-types-api-openapi.yml
- filename: astrocal-dev-organizations-api-openapi.yml
  format: yaml
  label: Astrocal Organizations API
  slug: astrocal-dev-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astrocal-dev/openapi/astrocal-dev-organizations-api-openapi.yml
- filename: astrocal-dev-payments-api-openapi.yml
  format: yaml
  label: Astrocal Payments API
  slug: astrocal-dev-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astrocal-dev/openapi/astrocal-dev-payments-api-openapi.yml
- filename: astrocal-dev-stripe-api-openapi.yml
  format: yaml
  label: Astrocal Stripe API
  slug: astrocal-dev-stripe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astrocal-dev/openapi/astrocal-dev-stripe-api-openapi.yml
- filename: astrocal-dev-subscription-api-openapi.yml
  format: yaml
  label: Astrocal Subscription API
  slug: astrocal-dev-subscription-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astrocal-dev/openapi/astrocal-dev-subscription-api-openapi.yml
- filename: astrocal-dev-support-api-openapi.yml
  format: yaml
  label: Astrocal Support API
  slug: astrocal-dev-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astrocal-dev/openapi/astrocal-dev-support-api-openapi.yml
- filename: astrocal-dev-team-api-openapi.yml
  format: yaml
  label: Astrocal Team API
  slug: astrocal-dev-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astrocal-dev/openapi/astrocal-dev-team-api-openapi.yml
- filename: astrocal-dev-test-data-api-openapi.yml
  format: yaml
  label: Astrocal Test Data API
  slug: astrocal-dev-test-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astrocal-dev/openapi/astrocal-dev-test-data-api-openapi.yml
- filename: astrocal-dev-usage-api-openapi.yml
  format: yaml
  label: Astrocal Usage API
  slug: astrocal-dev-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astrocal-dev/openapi/astrocal-dev-usage-api-openapi.yml
- filename: astrocal-dev-waitlist-api-openapi.yml
  format: yaml
  label: Astrocal Waitlist API
  slug: astrocal-dev-waitlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astrocal-dev/openapi/astrocal-dev-waitlist-api-openapi.yml
- filename: astrocal-dev-webhooks-api-openapi.yml
  format: yaml
  label: Astrocal Webhooks API
  slug: astrocal-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astrocal-dev/openapi/astrocal-dev-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Astrocal Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Astrocal declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Astrocal
provider_slug: astrocal-dev
scheme_count: 2
schemes:
- description: API key authentication using Bearer token in Authorization header.
  in: header
  name: Authorization
  scheme: bearer
  type: http
- additionalHeaders:
  - description: Organization UUID to act on behalf of.
    name: X-Org-Id
  - description: live (default) or test to control sandbox isolation.
    name: X-Astrocal-Mode
  description: Service key authentication for server-to-server use, with additional X-Org-Id and X-Astrocal-Mode headers.
  in: header
  name: Authorization
  scheme: bearer
  type: http
slug: astrocal-dev-authentication
source_filename: astrocal-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://www.astrocal.dev/docs/guides/authentication\nschemes:\n  - type: http\n    scheme: bearer\n    description: API key authentication using Bearer token in Authorization header.\n    name: Authorization\n    in: header\n  - type: http\n    scheme: bearer\n    description: Service key authentication for server-to-server use, with additional X-Org-Id and X-Astrocal-Mode headers.\n    name: Authorization\n    in: header\n    additionalHeaders:\n      - name: X-Org-Id\n        description: Organization UUID to act on behalf of.\n      - name: X-Astrocal-Mode\n        description: live (default) or test to control sandbox isolation.\n"
source_yaml_url: https://artifacts.apis.io/astrocal-dev/authentication/astrocal-dev-authentication.yml
summary_line: 2 schemes
tags:
- Scheduling
- Booking
- Small Business
- Payments
---
