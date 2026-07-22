---
api_key_in: []
auth_types:
- apiKey
description: TrueCoach publishes no public developer API program or API reference, so there is no OpenAPI to derive an auth profile from. The only documented programmatic access is the Zapier partner integration (Pro plan and above), authorized with an API key that a coach copies from Settings > Integration > Zapier (app.truecoach.co/coach/account/trainer-zapier) and pastes into Zapier. The web/mobile apps themselves authenticate end users with email/password and Google OAuth 2.0 sign-in against the private api.truecoach.co backend; that surface is not documented for third parties.
kind: authentication
layout: security
method: searched
name: Truecoach Authentication
name_suffix: Authentication
oauth_flows: []
overview: TrueCoach secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TrueCoach
provider_slug: truecoach
scheme_count: 1
schemes:
- description: Per-account API key issued in the TrueCoach coach settings (Settings > Integration > Zapier) and used to authorize the TrueCoach app inside Zapier. Key placement (header/param) is handled by the Zapier connector and is not publicly documented.
  docs: https://help.truecoach.co/en/articles/8688374-zapier-integration
  name: zapierApiKey
  sources:
  - https://help.truecoach.co/en/articles/8688374-zapier-integration
  type: apiKey
slug: truecoach-authentication
source_filename: truecoach-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://help.truecoach.co/en/articles/8688374-zapier-integration\ndocs: https://help.truecoach.co/en/articles/8688374-zapier-integration\ndescription: >-\n  TrueCoach publishes no public developer API program or API reference, so\n  there is no OpenAPI to derive an auth profile from. The only documented\n  programmatic access is the Zapier partner integration (Pro plan and above),\n  authorized with an API key that a coach copies from Settings > Integration >\n  Zapier (app.truecoach.co/coach/account/trainer-zapier) and pastes into\n  Zapier. The web/mobile apps themselves authenticate end users with\n  email/password and Google OAuth 2.0 sign-in against the private\n  api.truecoach.co backend; that surface is not documented for third parties.\nsummary:\n  types:\n    - apiKey\n  notes:\n    - No public API reference; API key is only documented for the Zapier connector.\n    - Zapier access is gated to the Pro plan and above.\n\
  schemes:\n  - name: zapierApiKey\n    type: apiKey\n    description: >-\n      Per-account API key issued in the TrueCoach coach settings (Settings >\n      Integration > Zapier) and used to authorize the TrueCoach app inside\n      Zapier. Key placement (header/param) is handled by the Zapier connector\n      and is not publicly documented.\n    docs: https://help.truecoach.co/en/articles/8688374-zapier-integration\n    sources:\n      - https://help.truecoach.co/en/articles/8688374-zapier-integration\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truecoach/refs/heads/main/authentication/truecoach-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fitness
- Personal Training
- Coaching
- Workouts
- Nutrition
- Health
- SaaS
---
