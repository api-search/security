---
anonymous_access: false
api_key_in: []
api_specs:
- filename: concord-com-webhooks-api-openapi.yml
  format: yaml
  label: Concord Webhooks (Outbound Events)
  slug: concord-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/concord-com/openapi/concord-com-webhooks-api-openapi.yml
- filename: concord-com-agreement-api-openapi.yml
  format: yaml
  label: Concord Agreement API
  slug: concord-com-agreement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/concord-com/openapi/concord-com-agreement-api-openapi.yml
- filename: concord-com-agreement-versions-api-openapi.yml
  format: yaml
  label: Concord Agreement Versions API
  slug: concord-com-agreement-versions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/concord-com/openapi/concord-com-agreement-versions-api-openapi.yml
- filename: concord-com-automated-template-api-openapi.yml
  format: yaml
  label: Concord Automated Template API
  slug: concord-com-automated-template-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/concord-com/openapi/concord-com-automated-template-api-openapi.yml
- filename: concord-com-clause-library-api-openapi.yml
  format: yaml
  label: Concord Clause Library API
  slug: concord-com-clause-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/concord-com/openapi/concord-com-clause-library-api-openapi.yml
- filename: concord-com-custom-branding-api-openapi.yml
  format: yaml
  label: Concord Custom Branding API
  slug: concord-com-custom-branding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/concord-com/openapi/concord-com-custom-branding-api-openapi.yml
- filename: concord-com-events-api-openapi.yml
  format: yaml
  label: Concord Events API
  slug: concord-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/concord-com/openapi/concord-com-events-api-openapi.yml
- filename: concord-com-folders-api-openapi.yml
  format: yaml
  label: Concord Folders API
  slug: concord-com-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/concord-com/openapi/concord-com-folders-api-openapi.yml
- filename: concord-com-organization-api-openapi.yml
  format: yaml
  label: Concord Organization API
  slug: concord-com-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/concord-com/openapi/concord-com-organization-api-openapi.yml
- filename: concord-com-organization-groups-api-openapi.yml
  format: yaml
  label: Concord Organization Groups API
  slug: concord-com-organization-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/concord-com/openapi/concord-com-organization-groups-api-openapi.yml
- filename: concord-com-organization-invitation-api-openapi.yml
  format: yaml
  label: Concord Organization invitation API
  slug: concord-com-organization-invitation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/concord-com/openapi/concord-com-organization-invitation-api-openapi.yml
- filename: concord-com-organization-members-api-openapi.yml
  format: yaml
  label: Concord Organization Members API
  slug: concord-com-organization-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/concord-com/openapi/concord-com-organization-members-api-openapi.yml
- filename: concord-com-report-api-openapi.yml
  format: yaml
  label: Concord Report API
  slug: concord-com-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/concord-com/openapi/concord-com-report-api-openapi.yml
- filename: concord-com-signature-api-openapi.yml
  format: yaml
  label: Concord Signature API
  slug: concord-com-signature-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/concord-com/openapi/concord-com-signature-api-openapi.yml
- filename: concord-com-tags-api-openapi.yml
  format: yaml
  label: Concord Tags API
  slug: concord-com-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/concord-com/openapi/concord-com-tags-api-openapi.yml
- filename: concord-com-user-api-openapi.yml
  format: yaml
  label: Concord User API
  slug: concord-com-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/concord-com/openapi/concord-com-user-api-openapi.yml
- filename: concord-com-user-integrations-api-openapi.yml
  format: yaml
  label: Concord User integrations API
  slug: concord-com-user-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/concord-com/openapi/concord-com-user-integrations-api-openapi.yml
- filename: concord-com-webhooks-api-openapi.yml
  format: yaml
  label: Concord Webhooks API
  slug: concord-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/concord-com/openapi/concord-com-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Concord Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Concord secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Concord
provider_slug: concord-com
scheme_count: 1
schemes:
- description: API key generated inside the Concord account (paid plans only) and sent in the `X-API-KEY` request header. Confirmed against the live production host https://api.concordnow.com/api/rest/1, which returns HTTP 401 `{"statusCode":401,"restCode":"unauthorized"}` when called without a valid key.
  in: header
  keyName: X-API-KEY
  name: apiKeyAuth
  sources:
  - openapi/concord-com-openapi.yml
  - https://help.concord.app/concord-api
  type: apiKey
slug: concord-com-authentication
source_filename: concord-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/concord-com-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  keyName: X-API-KEY\n  description: >-\n    API key generated inside the Concord account (paid plans only) and sent in\n    the `X-API-KEY` request header. Confirmed against the live production host\n    https://api.concordnow.com/api/rest/1, which returns HTTP 401\n    `{\"statusCode\":401,\"restCode\":\"unauthorized\"}` when called without a valid\n    key.\n  sources:\n  - openapi/concord-com-openapi.yml\n  - https://help.concord.app/concord-api\n"
source_yaml_url: https://artifacts.apis.io/concord-com/authentication/concord-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Contract Management
- Contract Lifecycle Management
- Contracts
- Agreements
- E-Signature
- Document Management
- Legal
- Workflows
---
