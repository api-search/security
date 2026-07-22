---
api_key_in:
- header
api_specs:
- filename: wunderkind-email-openapi.yml
  format: yaml
  label: Wunderkind Email API
  slug: wunderkind-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wunderkind/refs/heads/main/openapi/wunderkind-email-openapi.yml
- filename: wunderkind-identity-openapi.yml
  format: yaml
  label: Wunderkind Identity API
  slug: wunderkind-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wunderkind/refs/heads/main/openapi/wunderkind-identity-openapi.yml
- filename: wunderkind-ucrm-openapi.yml
  format: yaml
  label: Wunderkind UCRM API
  slug: wunderkind-ucrm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wunderkind/refs/heads/main/openapi/wunderkind-ucrm-openapi.yml
- filename: wunderkind-event-ingestion-openapi.yml
  format: yaml
  label: Wunderkind Event Ingestion API
  slug: wunderkind-event-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wunderkind/refs/heads/main/openapi/wunderkind-event-ingestion-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Wunderkind Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wunderkind secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Wunderkind
provider_slug: wunderkind
scheme_count: 4
schemes:
- description: Private API key created in Wunderkind Platform (Settings > API Credentials), scoped to an API product such as id-resolution or UCRM. Never use private keys in client-side code or public repositories.
  docs: https://developer.wunderkind.co/docs/authenticate-api-requests
  format: apikey {apikey}
  hosts:
  - https://api.wunderkind.co
  in: header
  name: PrivateApiKey
  parameter: Authorization
  sources:
  - openapi/wunderkind-identity-openapi.yml
  - openapi/wunderkind-ucrm-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: Bearer token authentication documented for the Wunderkind Email API.
  hosts:
  - https://api.wunderkind.co
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/wunderkind-email-openapi.yml
  type: http
- description: Paired headers for the Text Message API on api.wknd.ai; X-Client-ID is a 32-byte hashed string and X-Client-Secret a 64-byte hashed string, both provided by Wunderkind.
  docs: https://developer.wunderkind.co/reference/text-message-api
  hosts:
  - https://api.wknd.ai
  in: header
  name: TextApiClientCredentials
  parameter: X-Client-ID / X-Client-Secret
  type: apiKey
- description: Public key authentication for client-side endpoints on api.bounceexchange.com; the public API key is the numeric website ID (site ID), normally handled by the Web and Mobile SDKs.
  docs: https://developer.wunderkind.co/docs/authenticate-api-requests
  hosts:
  - https://api.bounceexchange.com
  in: query
  name: PublicSiteId
  parameter: website_id
  type: apiKey
slug: wunderkind-authentication
source_filename: wunderkind-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.wunderkind.co/docs/authenticate-api-requests\ndocs: https://developer.wunderkind.co/docs/authenticate-api-requests\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  notes: >-\n    Wunderkind splits authentication by surface. Server-side APIs on\n    api.wunderkind.co authenticate with a private API key sent as\n    \"Authorization: apikey {apikey}\"; keys are created per API product\n    (id-resolution, UCRM, ...) under Settings > API Credentials in Wunderkind\n    Platform and require an Admin or Manager role. Client-side APIs on\n    api.bounceexchange.com use a public key: the numeric website ID (site ID),\n    normally supplied via the Mobile/Web SDKs. The Text Message API on\n    api.wknd.ai uses paired X-Client-ID / X-Client-Secret headers provisioned\n    by Wunderkind. The Email API documents Bearer (JWT) token authentication.\n    A 400 error indicates an invalid or missing API\
  \ key on server-side\n    endpoints.\nschemes:\n- name: PrivateApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'apikey {apikey}'\n  description: >-\n    Private API key created in Wunderkind Platform (Settings > API\n    Credentials), scoped to an API product such as id-resolution or UCRM.\n    Never use private keys in client-side code or public repositories.\n  hosts:\n  - https://api.wunderkind.co\n  sources:\n  - openapi/wunderkind-identity-openapi.yml\n  - openapi/wunderkind-ucrm-openapi.yml\n  docs: https://developer.wunderkind.co/docs/authenticate-api-requests\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token authentication documented for the Wunderkind Email API.\n  hosts:\n  - https://api.wunderkind.co\n  sources:\n  - openapi/wunderkind-email-openapi.yml\n- name: TextApiClientCredentials\n  type: apiKey\n  in: header\n  parameter: X-Client-ID / X-Client-Secret\n  description: >-\n    Paired headers\
  \ for the Text Message API on api.wknd.ai; X-Client-ID is a\n    32-byte hashed string and X-Client-Secret a 64-byte hashed string, both\n    provided by Wunderkind.\n  hosts:\n  - https://api.wknd.ai\n  docs: https://developer.wunderkind.co/reference/text-message-api\n- name: PublicSiteId\n  type: apiKey\n  in: query\n  parameter: website_id\n  description: >-\n    Public key authentication for client-side endpoints on\n    api.bounceexchange.com; the public API key is the numeric website ID\n    (site ID), normally handled by the Web and Mobile SDKs.\n  hosts:\n  - https://api.bounceexchange.com\n  docs: https://developer.wunderkind.co/docs/authenticate-api-requests\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wunderkind/refs/heads/main/authentication/wunderkind-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Company
- Marketing
- Personalization
- Identity Resolution
- Email
- SMS
- Behavioral Data
- eCommerce
- Webhooks
---
