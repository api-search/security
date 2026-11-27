---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nuance-application-configurations-api-openapi.yml
  format: yaml
  label: Nuance Application Configurations API
  slug: nuance-application-configurations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance/openapi/nuance-application-configurations-api-openapi.yml
- filename: nuance-applications-api-openapi.yml
  format: yaml
  label: Nuance Applications API
  slug: nuance-applications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance/openapi/nuance-applications-api-openapi.yml
- filename: nuance-bots-api-openapi.yml
  format: yaml
  label: Nuance Bots API
  slug: nuance-bots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance/openapi/nuance-bots-api-openapi.yml
- filename: nuance-builds-api-openapi.yml
  format: yaml
  label: Nuance Builds API
  slug: nuance-builds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance/openapi/nuance-builds-api-openapi.yml
- filename: nuance-data-hosts-api-openapi.yml
  format: yaml
  label: Nuance Data Hosts API
  slug: nuance-data-hosts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance/openapi/nuance-data-hosts-api-openapi.yml
- filename: nuance-data-types-api-openapi.yml
  format: yaml
  label: Nuance Data Types API
  slug: nuance-data-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance/openapi/nuance-data-types-api-openapi.yml
- filename: nuance-deployment-flows-api-openapi.yml
  format: yaml
  label: Nuance Deployment Flows API
  slug: nuance-deployment-flows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance/openapi/nuance-deployment-flows-api-openapi.yml
- filename: nuance-engine-packs-api-openapi.yml
  format: yaml
  label: Nuance Engine Packs API
  slug: nuance-engine-packs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance/openapi/nuance-engine-packs-api-openapi.yml
- filename: nuance-entities-api-openapi.yml
  format: yaml
  label: Nuance Entities API
  slug: nuance-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance/openapi/nuance-entities-api-openapi.yml
- filename: nuance-environment-configurations-api-openapi.yml
  format: yaml
  label: Nuance Environment Configurations API
  slug: nuance-environment-configurations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance/openapi/nuance-environment-configurations-api-openapi.yml
- filename: nuance-environments-api-openapi.yml
  format: yaml
  label: Nuance Environments API
  slug: nuance-environments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance/openapi/nuance-environments-api-openapi.yml
- filename: nuance-geographies-api-openapi.yml
  format: yaml
  label: Nuance Geographies API
  slug: nuance-geographies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance/openapi/nuance-geographies-api-openapi.yml
- filename: nuance-intents-api-openapi.yml
  format: yaml
  label: Nuance Intents API
  slug: nuance-intents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance/openapi/nuance-intents-api-openapi.yml
- filename: nuance-jobs-api-openapi.yml
  format: yaml
  label: Nuance Jobs API
  slug: nuance-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance/openapi/nuance-jobs-api-openapi.yml
- filename: nuance-language-topics-api-openapi.yml
  format: yaml
  label: Nuance Language Topics API
  slug: nuance-language-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance/openapi/nuance-language-topics-api-openapi.yml
- filename: nuance-ontology-api-openapi.yml
  format: yaml
  label: Nuance Ontology API
  slug: nuance-ontology-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance/openapi/nuance-ontology-api-openapi.yml
- filename: nuance-organizations-api-openapi.yml
  format: yaml
  label: Nuance Organizations API
  slug: nuance-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance/openapi/nuance-organizations-api-openapi.yml
- filename: nuance-projects-api-openapi.yml
  format: yaml
  label: Nuance Projects API
  slug: nuance-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance/openapi/nuance-projects-api-openapi.yml
- filename: nuance-samples-api-openapi.yml
  format: yaml
  label: Nuance Samples API
  slug: nuance-samples-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance/openapi/nuance-samples-api-openapi.yml
- filename: nuance-snapshots-api-openapi.yml
  format: yaml
  label: Nuance Snapshots API
  slug: nuance-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance/openapi/nuance-snapshots-api-openapi.yml
- filename: nuance-version-api-openapi.yml
  format: yaml
  label: Nuance Version API
  slug: nuance-version-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance/openapi/nuance-version-api-openapi.yml
- filename: nuance-versions-api-openapi.yml
  format: yaml
  label: Nuance Versions API
  slug: nuance-versions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance/openapi/nuance-versions-api-openapi.yml
- filename: nuance-voices-api-openapi.yml
  format: yaml
  label: Nuance Voices API
  slug: nuance-voices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuance/openapi/nuance-voices-api-openapi.yml
auth_types:
- oauth2
description: Nuance Mix runtime services (ASRaaS, NLUaaS, DLGaaS, TTSaaS, NRaaS) and the Mix V4 authoring API authenticate with OAuth 2.0 using the client-credentials grant. Developers generate a service-credentials client (client id + secret) in the Mix dashboard, exchange it for a short-lived bearer access token at the Nuance authorization server, and present the token to the gRPC runtime over a TLS-secured channel. Access is scoped per runtime service.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Nuance Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Nuance secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Nuance
provider_slug: nuance
scheme_count: 1
schemes:
- description: OAuth 2.0 client-credentials grant. The access token is presented as a Bearer credential on the gRPC call metadata; tokens are short-lived and refreshed by the client. Service credentials are created and managed in the Mix dashboard (mix.nuance.com).
  flow: clientCredentials
  grant: client_credentials
  name: MixOAuth2
  scoped_services:
  - asr
  - nlu
  - dlg
  - tts
  - nr
  sources:
  - docs.nuance.com/mix
  token_style: bearer
  type: oauth2
slug: nuance-authentication
source_filename: nuance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.nuance.com/mix/apis/\ndocs: https://docs.nuance.com/mix/\ndescription: >-\n  Nuance Mix runtime services (ASRaaS, NLUaaS, DLGaaS, TTSaaS, NRaaS) and the\n  Mix V4 authoring API authenticate with OAuth 2.0 using the client-credentials\n  grant. Developers generate a service-credentials client (client id + secret)\n  in the Mix dashboard, exchange it for a short-lived bearer access token at the\n  Nuance authorization server, and present the token to the gRPC runtime over a\n  TLS-secured channel. Access is scoped per runtime service.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  transport: grpc-tls\nschemes:\n  - name: MixOAuth2\n    type: oauth2\n    flow: clientCredentials\n    grant: client_credentials\n    token_style: bearer\n    description: >-\n      OAuth 2.0 client-credentials grant. The access token is presented as a\n      Bearer credential on the gRPC call metadata; tokens are\
  \ short-lived and\n      refreshed by the client. Service credentials are created and managed in\n      the Mix dashboard (mix.nuance.com).\n    scoped_services: [asr, nlu, dlg, tts, nr]\n    sources: [docs.nuance.com/mix]\nnotes: >-\n  Scope tokens are assigned per runtime service in the Mix dashboard; exact\n  scope strings are managed there and were not captured verbatim (the docs are\n  a client-rendered SPA). See scopes handling in docs.nuance.com/mix/apis/.\n"
source_yaml_url: https://artifacts.apis.io/nuance/authentication/nuance-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Speech Recognition
- Conversational AI
- Natural Language Understanding
- Text-to-Speech
- Speech Synthesis
- Voice
- Dialog
- gRPC
- Healthcare AI
---
