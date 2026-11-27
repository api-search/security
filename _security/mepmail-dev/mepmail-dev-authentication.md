---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mepmail-dev-account-api-openapi.yml
  format: yaml
  label: MepMail Account API
  slug: mepmail-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-account-api-openapi.yml
- filename: mepmail-dev-api-keys-api-openapi.yml
  format: yaml
  label: MepMail API keys API
  slug: mepmail-dev-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-api-keys-api-openapi.yml
- filename: mepmail-dev-audiences-api-openapi.yml
  format: yaml
  label: MepMail Audiences API
  slug: mepmail-dev-audiences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-audiences-api-openapi.yml
- filename: mepmail-dev-broadcasts-api-openapi.yml
  format: yaml
  label: MepMail Broadcasts API
  slug: mepmail-dev-broadcasts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-broadcasts-api-openapi.yml
- filename: mepmail-dev-contact-properties-api-openapi.yml
  format: yaml
  label: MepMail Contact properties API
  slug: mepmail-dev-contact-properties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-contact-properties-api-openapi.yml
- filename: mepmail-dev-contacts-api-openapi.yml
  format: yaml
  label: MepMail Contacts API
  slug: mepmail-dev-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-contacts-api-openapi.yml
- filename: mepmail-dev-domains-api-openapi.yml
  format: yaml
  label: MepMail Domains API
  slug: mepmail-dev-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-domains-api-openapi.yml
- filename: mepmail-dev-emails-api-openapi.yml
  format: yaml
  label: MepMail Emails API
  slug: mepmail-dev-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-emails-api-openapi.yml
- filename: mepmail-dev-segments-api-openapi.yml
  format: yaml
  label: MepMail Segments API
  slug: mepmail-dev-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-segments-api-openapi.yml
- filename: mepmail-dev-suppressions-api-openapi.yml
  format: yaml
  label: MepMail Suppressions API
  slug: mepmail-dev-suppressions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-suppressions-api-openapi.yml
- filename: mepmail-dev-templates-api-openapi.yml
  format: yaml
  label: MepMail Templates API
  slug: mepmail-dev-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-templates-api-openapi.yml
- filename: mepmail-dev-topics-api-openapi.yml
  format: yaml
  label: MepMail Topics API
  slug: mepmail-dev-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-topics-api-openapi.yml
- filename: mepmail-dev-webhooks-api-openapi.yml
  format: yaml
  label: MepMail Webhooks API
  slug: mepmail-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mepmail-dev/openapi/mepmail-dev-webhooks-api-openapi.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: MepMail Authentication
name_suffix: Authentication
oauth_flows: []
overview: MepMail declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MepMail
provider_slug: mepmail-dev
scheme_count: 1
schemes:
- evidence: 'authenticate with `Authorization: Bearer ms_...`.'
  header: Authorization
  location: header
  name: Bearer token
  type: http-bearer
slug: mepmail-dev-authentication
source_filename: mepmail-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.mepmail.dev/api-reference/endpoints/api-keys/get.md
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.mepmail.dev/api-reference/endpoints/api-keys/get.md\nsources:\n- https://docs.mepmail.dev/api-reference/endpoints/api-keys/get.md\n- https://docs.mepmail.dev/api-reference/endpoints/api-keys/post.md\n- https://docs.mepmail.dev/api-reference/endpoints/api-keys/id/delete.md\n- https://docs.mepmail.dev/api-reference/endpoints/webhooks/id/rotate/post.md\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'authenticate with `Authorization: Bearer ms_...`.'\n  location: header\n  header: Authorization\ndocs: https://docs.mepmail.dev/api-reference/endpoints/api-keys/get.md\n"
source_yaml_url: https://artifacts.apis.io/mepmail-dev/authentication/mepmail-dev-authentication.yml
summary_line: 1 scheme
tags:
- Email
- Services
- Communications
- Developers
---
