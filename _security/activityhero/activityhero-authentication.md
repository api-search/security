---
api_key_in: []
auth_types:
- signature
description: ActivityHero's provider integration (Registration API and Schedule API) does not use API keys, OAuth, or bearer tokens for its request/response surface. Instead, webhook payloads are authenticated with an HMAC-SHA256 signature so the receiver can verify the message originated from ActivityHero (and, symmetrically, so ActivityHero can verify inbound schedule syncs).
kind: authentication
layout: security
method: searched
name: Activityhero Authentication
name_suffix: Authentication
oauth_flows: []
overview: ActivityHero secures its APIs with signature across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ActivityHero
provider_slug: activityhero
scheme_count: 1
schemes:
- algorithm: HMAC-SHA256
  header: Signature
  message: '"providerID_timestamp" (provider ID and request timestamp joined by an underscore)'
  name: hmacSignature
  reference: https://hookdeck.com/webhooks/guides/how-to-implement-sha256-webhook-signature-verification
  secret_location: A per-provider secret key found in the Registration API dashboard section (Manage Listing > API).
  sources:
  - https://help.activityhero.com/can-i-sync-activityhero-registrations-to-my-own-database
  - https://help.activityhero.com/can-i-sync-my-activity-schedules-into-activityhero
  type: signature
  verification: The receiver recomputes HMAC-SHA256 over "providerID_timestamp" using the shared secret and compares it to the Signature header.
slug: activityhero-authentication
source_filename: activityhero-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: >-\n  https://help.activityhero.com/can-i-sync-activityhero-registrations-to-my-own-database ,\n  https://help.activityhero.com/can-i-sync-my-activity-schedules-into-activityhero\ndescription: >-\n  ActivityHero's provider integration (Registration API and Schedule API) does\n  not use API keys, OAuth, or bearer tokens for its request/response surface.\n  Instead, webhook payloads are authenticated with an HMAC-SHA256 signature so\n  the receiver can verify the message originated from ActivityHero (and,\n  symmetrically, so ActivityHero can verify inbound schedule syncs).\nsummary:\n  types:\n    - signature\nschemes:\n  - name: hmacSignature\n    type: signature\n    algorithm: HMAC-SHA256\n    header: Signature\n    message: '\"providerID_timestamp\" (provider ID and request timestamp joined by an underscore)'\n    secret_location: >-\n      A per-provider secret key found in the Registration API dashboard\n      section\
  \ (Manage Listing > API).\n    verification: >-\n      The receiver recomputes HMAC-SHA256 over \"providerID_timestamp\" using the\n      shared secret and compares it to the Signature header.\n    reference: https://hookdeck.com/webhooks/guides/how-to-implement-sha256-webhook-signature-verification\n    sources:\n      - https://help.activityhero.com/can-i-sync-activityhero-registrations-to-my-own-database\n      - https://help.activityhero.com/can-i-sync-my-activity-schedules-into-activityhero\ndocs: https://help.activityhero.com/api\nnotes:\n  - No OAuth2 or OpenID Connect flow is published.\n  - No API-key header is used; trust is established via the shared HMAC secret and the Signature header.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/activityhero/refs/heads/main/authentication/activityhero-authentication.yml
summary_line: signature · 1 scheme
tags:
- Company
- Kids Activities
- Camps
- Classes
- Marketplace
- Registration
- Webhooks
- Education
---
