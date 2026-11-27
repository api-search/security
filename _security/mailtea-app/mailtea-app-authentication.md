---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mailtea-app-api-keys-api-openapi.yml
  format: yaml
  label: Mailtea API keys API
  slug: mailtea-app-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtea-app/openapi/mailtea-app-api-keys-api-openapi.yml
- filename: mailtea-app-assets-api-openapi.yml
  format: yaml
  label: Mailtea Assets API
  slug: mailtea-app-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtea-app/openapi/mailtea-app-assets-api-openapi.yml
- filename: mailtea-app-automation-runs-api-openapi.yml
  format: yaml
  label: Mailtea Automation Runs API
  slug: mailtea-app-automation-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtea-app/openapi/mailtea-app-automation-runs-api-openapi.yml
- filename: mailtea-app-automations-api-openapi.yml
  format: yaml
  label: Mailtea Automations API
  slug: mailtea-app-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtea-app/openapi/mailtea-app-automations-api-openapi.yml
- filename: mailtea-app-contact-properties-api-openapi.yml
  format: yaml
  label: Mailtea Contact properties API
  slug: mailtea-app-contact-properties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtea-app/openapi/mailtea-app-contact-properties-api-openapi.yml
- filename: mailtea-app-contacts-api-openapi.yml
  format: yaml
  label: Mailtea Contacts API
  slug: mailtea-app-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtea-app/openapi/mailtea-app-contacts-api-openapi.yml
- filename: mailtea-app-domains-api-openapi.yml
  format: yaml
  label: Mailtea Domains API
  slug: mailtea-app-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtea-app/openapi/mailtea-app-domains-api-openapi.yml
- filename: mailtea-app-emails-api-openapi.yml
  format: yaml
  label: Mailtea Emails API
  slug: mailtea-app-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtea-app/openapi/mailtea-app-emails-api-openapi.yml
- filename: mailtea-app-events-api-openapi.yml
  format: yaml
  label: Mailtea Events API
  slug: mailtea-app-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtea-app/openapi/mailtea-app-events-api-openapi.yml
- filename: mailtea-app-inbound-email-api-openapi.yml
  format: yaml
  label: Mailtea Inbound email API
  slug: mailtea-app-inbound-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtea-app/openapi/mailtea-app-inbound-email-api-openapi.yml
- filename: mailtea-app-posts-api-openapi.yml
  format: yaml
  label: Mailtea Posts API
  slug: mailtea-app-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtea-app/openapi/mailtea-app-posts-api-openapi.yml
- filename: mailtea-app-segments-api-openapi.yml
  format: yaml
  label: Mailtea Segments API
  slug: mailtea-app-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtea-app/openapi/mailtea-app-segments-api-openapi.yml
- filename: mailtea-app-senders-api-openapi.yml
  format: yaml
  label: Mailtea Senders API
  slug: mailtea-app-senders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtea-app/openapi/mailtea-app-senders-api-openapi.yml
- filename: mailtea-app-subscribe-api-openapi.yml
  format: yaml
  label: Mailtea Subscribe API
  slug: mailtea-app-subscribe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtea-app/openapi/mailtea-app-subscribe-api-openapi.yml
- filename: mailtea-app-suppressions-api-openapi.yml
  format: yaml
  label: Mailtea Suppressions API
  slug: mailtea-app-suppressions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtea-app/openapi/mailtea-app-suppressions-api-openapi.yml
- filename: mailtea-app-templates-api-openapi.yml
  format: yaml
  label: Mailtea Templates API
  slug: mailtea-app-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtea-app/openapi/mailtea-app-templates-api-openapi.yml
- filename: mailtea-app-topics-api-openapi.yml
  format: yaml
  label: Mailtea Topics API
  slug: mailtea-app-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtea-app/openapi/mailtea-app-topics-api-openapi.yml
- filename: mailtea-app-unsubscribe-api-openapi.yml
  format: yaml
  label: Mailtea Unsubscribe API
  slug: mailtea-app-unsubscribe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtea-app/openapi/mailtea-app-unsubscribe-api-openapi.yml
- filename: mailtea-app-webhooks-api-openapi.yml
  format: yaml
  label: Mailtea Webhooks API
  slug: mailtea-app-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtea-app/openapi/mailtea-app-webhooks-api-openapi.yml
auth_types: []
description: Mailtea API authentication uses Bearer tokens sent in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mailtea Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mailtea declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Mailtea
provider_slug: mailtea-app
scheme_count: 1
schemes:
- evidence: 'Send any token as a Bearer header:'
  header: Authorization
  how_to_obtain: Create a Personal Access Token (PAT), Service Key, or Test Key in Mailtea Studio (Settings > API Tokens) and copy the token.
  location: header
  name: Bearer
  type: http-bearer
slug: mailtea-app-authentication
source_filename: mailtea-app-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.mailtea.app/docs/api-reference/authentication
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.mailtea.app/docs/api-reference/authentication\nsources:\n- https://docs.mailtea.app/docs/api-reference/authentication\n- https://docs.mailtea.app/docs/api-reference/api-keys\n- https://docs.mailtea.app/docs/api-reference/api-keys/create-api-key\n- https://docs.mailtea.app/docs/api-reference/api-keys/list-api-keys\ndescription: Mailtea API authentication uses Bearer tokens sent in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send any token as a Bearer header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a Personal Access Token (PAT), Service Key, or Test Key in Mailtea Studio (Settings > API Tokens) and copy the token.\nnote: No OAuth2 flows are described; authentication is performed by providing the token directly as a Bearer header.\ndocs: https://docs.mailtea.app/docs/api-reference/authentication\n"
source_yaml_url: https://artifacts.apis.io/mailtea-app/authentication/mailtea-app-authentication.yml
summary_line: 1 scheme
tags:
- Email
- Artificial Intelligence
- Platform
- Developer Tools
- Marketing
---
