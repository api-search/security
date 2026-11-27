---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pagelens-io-openapi-generated.yml
  format: yaml
  label: PageLens API
  slug: pagelens-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelens-io/openapi/_ae-authored/pagelens-io-openapi-generated.yml
auth_types: []
description: Authentication for Stripe webhooks
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: PageLens Authentication
name_suffix: Authentication
oauth_flows: []
overview: PageLens declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: PageLens
provider_slug: pagelens-io
scheme_count: 1
schemes:
- evidence: Verify signatures. Check the Stripe-Signature header against your endpoint's signing secret, using the raw request body, and reject old timestamps.
  header: Stripe-Signature
  how_to_obtain: Provided by Stripe when configuring the webhook endpoint
  location: header
  name: Stripe signing secret
  type: apiKey
slug: pagelens-io-authentication
source_filename: pagelens-io-authentication.yml
source_heading: Authentication Profile
source_url: https://pagelens.io/blog/stripe-revenue-attribution-without-cookies
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://pagelens.io/blog/stripe-revenue-attribution-without-cookies\nsources:\n- https://pagelens.io/blog/stripe-revenue-attribution-without-cookies\ndescription: Authentication for Stripe webhooks\nschemes:\n- type: apiKey\n  name: Stripe signing secret\n  evidence: Verify signatures. Check the Stripe-Signature header against your endpoint's signing secret, using the raw request body, and reject\n    old timestamps.\n  location: header\n  header: Stripe-Signature\n  how_to_obtain: Provided by Stripe when configuring the webhook endpoint\ndocs: https://pagelens.io/blog/stripe-revenue-attribution-without-cookies\n"
source_yaml_url: https://artifacts.apis.io/pagelens-io/authentication/pagelens-io-authentication.yml
summary_line: 1 scheme
tags:
- Analytics
- Artificial Intelligence
- Privacy
- Cookieless
- Web Analytics
---
