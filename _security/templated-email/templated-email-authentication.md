---
anonymous_access: false
api_key_in: []
api_specs:
- filename: templated-email-accounts-api-openapi.yml
  format: yaml
  label: Templated Accounts API
  slug: templated-email-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-accounts-api-openapi.yml
- filename: templated-email-ai-api-openapi.yml
  format: yaml
  label: Templated AI API
  slug: templated-email-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-ai-api-openapi.yml
- filename: templated-email-api-keys-api-openapi.yml
  format: yaml
  label: Templated API Keys API
  slug: templated-email-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-api-keys-api-openapi.yml
- filename: templated-email-brand-kit-api-openapi.yml
  format: yaml
  label: Templated Brand Kit API
  slug: templated-email-brand-kit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-brand-kit-api-openapi.yml
- filename: templated-email-fonts-api-openapi.yml
  format: yaml
  label: Templated Fonts API
  slug: templated-email-fonts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-fonts-api-openapi.yml
- filename: templated-email-images-api-openapi.yml
  format: yaml
  label: Templated Images API
  slug: templated-email-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-images-api-openapi.yml
- filename: templated-email-integrations-api-openapi.yml
  format: yaml
  label: Templated Integrations API
  slug: templated-email-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-integrations-api-openapi.yml
- filename: templated-email-members-api-openapi.yml
  format: yaml
  label: Templated Members API
  slug: templated-email-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-members-api-openapi.yml
- filename: templated-email-templates-api-openapi.yml
  format: yaml
  label: Templated Templates API
  slug: templated-email-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-templates-api-openapi.yml
- filename: templated-email-testing-api-openapi.yml
  format: yaml
  label: Templated Testing API
  slug: templated-email-testing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-testing-api-openapi.yml
- filename: templated-email-unsplash-api-openapi.yml
  format: yaml
  label: Templated Unsplash API
  slug: templated-email-unsplash-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-unsplash-api-openapi.yml
- filename: templated-email-subaccounts-api-openapi.yml
  format: yaml
  label: Templated Subaccounts API
  slug: templated-email-subaccounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/templated-email/openapi/templated-email-subaccounts-api-openapi.yml
auth_types: []
description: Authentication methods for the Templated API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Templated Authentication
name_suffix: Authentication
oauth_flows: []
overview: Templated declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Templated
provider_slug: templated-email
scheme_count: 2
schemes:
- evidence: 'Send them in the Authorization header: curl https://app.templated.email/api/accounts/{slug}/templates \ -H "Authorization: Bearer tmpl_sk_your_key_here"'
  header: Authorization
  how_to_obtain: Create a key in the app under Integrations → API Keys; the key is shown once at creation.
  location: header
  name: API Key
  type: http-bearer
- evidence: When a user signs in through the Templated web app, a session cookie (NextAuth.js) is set automatically.
  how_to_obtain: Sign in through the Templated web app; the session cookie is set automatically.
  location: cookie
  name: Session Cookie
  type: other
slug: templated-email-authentication
source_filename: templated-email-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.templated.email/docs/getting-started/authentication
source_yaml: "generated: '2026-11-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.templated.email/docs/getting-started/authentication\nsources:\n- https://developer.templated.email/docs/getting-started/authentication\n- https://developer.templated.email/docs/getting-started/overview\n- https://developer.templated.email/docs/getting-started/quickstart\n- https://developer.templated.email/docs/getting-started/rate-limits\ndescription: Authentication methods for the Templated API\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Send them in the Authorization header: curl https://app.templated.email/api/accounts/{slug}/templates \\ -H \"Authorization: Bearer\n    tmpl_sk_your_key_here\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the app under Integrations → API Keys; the key is shown once at creation.\n- type: other\n  name: Session Cookie\n  evidence: When a user signs in through the Templated web\
  \ app, a session cookie (NextAuth.js) is set automatically.\n  location: cookie\n  how_to_obtain: Sign in through the Templated web app; the session cookie is set automatically.\ndocs: https://developer.templated.email/docs/getting-started/authentication\n"
source_yaml_url: https://artifacts.apis.io/templated-email/authentication/templated-email-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Email
- AI
- No-code
- Marketing
---
