---
anonymous_access: false
api_key_in: []
api_specs:
- filename: joinblink-com-access-api-openapi.yml
  format: yaml
  label: Blink Access API
  slug: joinblink-com-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinblink-com/openapi/joinblink-com-access-api-openapi.yml
- filename: joinblink-com-chats-api-openapi.yml
  format: yaml
  label: Blink Chats API
  slug: joinblink-com-chats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinblink-com/openapi/joinblink-com-chats-api-openapi.yml
- filename: joinblink-com-feed-api-openapi.yml
  format: yaml
  label: Blink Feed API
  slug: joinblink-com-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinblink-com/openapi/joinblink-com-feed-api-openapi.yml
- filename: joinblink-com-forms-api-openapi.yml
  format: yaml
  label: Blink Forms API
  slug: joinblink-com-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinblink-com/openapi/joinblink-com-forms-api-openapi.yml
- filename: joinblink-com-group-api-openapi.yml
  format: yaml
  label: Blink Group API
  slug: joinblink-com-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinblink-com/openapi/joinblink-com-group-api-openapi.yml
- filename: joinblink-com-linked-account-api-openapi.yml
  format: yaml
  label: Blink Linked Account API
  slug: joinblink-com-linked-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinblink-com/openapi/joinblink-com-linked-account-api-openapi.yml
- filename: joinblink-com-linked-accounts-api-openapi.yml
  format: yaml
  label: Blink Linked Accounts API
  slug: joinblink-com-linked-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinblink-com/openapi/joinblink-com-linked-accounts-api-openapi.yml
- filename: joinblink-com-members-api-openapi.yml
  format: yaml
  label: Blink Members API
  slug: joinblink-com-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinblink-com/openapi/joinblink-com-members-api-openapi.yml
- filename: joinblink-com-messages-api-openapi.yml
  format: yaml
  label: Blink Messages API
  slug: joinblink-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinblink-com/openapi/joinblink-com-messages-api-openapi.yml
- filename: joinblink-com-user-api-openapi.yml
  format: yaml
  label: Blink User API
  slug: joinblink-com-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinblink-com/openapi/joinblink-com-user-api-openapi.yml
- filename: joinblink-com-service-provider-config-api-openapi.yml
  format: yaml
  label: Blink Service Provider Config API
  slug: joinblink-com-service-provider-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinblink-com/openapi/joinblink-com-service-provider-config-api-openapi.yml
auth_types: []
description: Authentication for Blink API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Joinblink Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blink declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Blink
provider_slug: joinblink-com
scheme_count: 1
schemes:
- evidence: The token you generate is a Bearer token so should be sent with every request to the API under the `Authorization` header as a value `Bearer <your token>`.
  header: Authorization
  how_to_obtain: Create an integration in the Blink Admin portal (Manage Apps) and generate a token for the app.
  location: header
  name: Bearer token
  type: http-bearer
slug: joinblink-com-authentication
source_filename: joinblink-com-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.joinblink.com/docs/creating-an-integration.md
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.joinblink.com/docs/creating-an-integration.md\nsources:\n- https://developer.joinblink.com/docs/creating-an-integration.md\n- https://developer.joinblink.com/docs/getting-started-with-blink-feed-api.md\n- https://developer.joinblink.com/reference/quick-start.md\n- https://developer.joinblink.com/reference/quick-start\ndescription: Authentication for Blink API\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: The token you generate is a Bearer token so should be sent with every request to the API under the `Authorization` header as a value\n    `Bearer <your token>`.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an integration in the Blink Admin portal (Manage Apps) and generate a token for the app.\ndocs: https://developer.joinblink.com/docs/creating-an-integration.md\n"
source_yaml_url: https://artifacts.apis.io/joinblink-com/authentication/joinblink-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- EmployeeExperience
- MobileFirst
- FrontlineWorkers
- Communication
---
