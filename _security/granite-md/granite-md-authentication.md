---
anonymous_access: false
api_key_in: []
api_specs:
- filename: granite-md-auth-api-openapi.yml
  format: yaml
  label: Granite Auth API
  slug: granite-md-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-auth-api-openapi.yml
- filename: granite-md-billing-api-openapi.yml
  format: yaml
  label: Granite Billing API
  slug: granite-md-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-billing-api-openapi.yml
- filename: granite-md-comments-api-openapi.yml
  format: yaml
  label: Granite Comments API
  slug: granite-md-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-comments-api-openapi.yml
- filename: granite-md-drive-api-openapi.yml
  format: yaml
  label: Granite Drive API
  slug: granite-md-drive-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-drive-api-openapi.yml
- filename: granite-md-folders-api-openapi.yml
  format: yaml
  label: Granite Folders API
  slug: granite-md-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-folders-api-openapi.yml
- filename: granite-md-knowledge-base-api-openapi.yml
  format: yaml
  label: Granite knowledge base API
  slug: granite-md-knowledge-base-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-knowledge-base-api-openapi.yml
- filename: granite-md-me-api-openapi.yml
  format: yaml
  label: Granite Me API
  slug: granite-md-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-me-api-openapi.yml
- filename: granite-md-meta-api-openapi.yml
  format: yaml
  label: Granite Meta API
  slug: granite-md-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-meta-api-openapi.yml
- filename: granite-md-note-shares-api-openapi.yml
  format: yaml
  label: Granite Note Shares API
  slug: granite-md-note-shares-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-note-shares-api-openapi.yml
- filename: granite-md-notes-api-openapi.yml
  format: yaml
  label: Granite Notes API
  slug: granite-md-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-notes-api-openapi.yml
- filename: granite-md-oauth-api-openapi.yml
  format: yaml
  label: Granite OAuth API
  slug: granite-md-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-oauth-api-openapi.yml
- filename: granite-md-publish-api-openapi.yml
  format: yaml
  label: Granite Publish API
  slug: granite-md-publish-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-publish-api-openapi.yml
- filename: granite-md-search-api-openapi.yml
  format: yaml
  label: Granite Search API
  slug: granite-md-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-search-api-openapi.yml
- filename: granite-md-shopify-api-openapi.yml
  format: yaml
  label: Granite Shopify API
  slug: granite-md-shopify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-shopify-api-openapi.yml
- filename: granite-md-sync-api-openapi.yml
  format: yaml
  label: Granite Sync API
  slug: granite-md-sync-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-sync-api-openapi.yml
- filename: granite-md-templates-api-openapi.yml
  format: yaml
  label: Granite Templates API
  slug: granite-md-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-templates-api-openapi.yml
- filename: granite-md-vaults-api-openapi.yml
  format: yaml
  label: Granite Vaults API
  slug: granite-md-vaults-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-vaults-api-openapi.yml
- filename: granite-md-webhooks-api-openapi.yml
  format: yaml
  label: Granite Webhooks API
  slug: granite-md-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-webhooks-api-openapi.yml
- filename: granite-md-workspaces-api-openapi.yml
  format: yaml
  label: Granite Workspaces API
  slug: granite-md-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/granite-md/openapi/granite-md-workspaces-api-openapi.yml
auth_types: []
description: Authentication methods described on Granite help pages.
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Granite Authentication
name_suffix: Authentication
oauth_flows: []
overview: Granite declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Granite
provider_slug: granite-md
scheme_count: 4
schemes:
- evidence: Sign in with your email and password, with Google, with Apple, or with your company's single sign-on.
  how_to_obtain: Sign up with your email and a password, or choose Continue with Google or Continue with Apple.
  name: Email and password
  type: http-basic
- evidence: Continue with Google Use your Google account.
  how_to_obtain: Continue with Google.
  name: Google
  type: oauth2
- evidence: Continue with Apple Use your Apple ID.
  how_to_obtain: Continue with Apple.
  name: Apple
  type: oauth2
- evidence: Continue with SSO For company workspaces that use Okta, Microsoft Entra ID, Google Workspace, or another identity provider.
  how_to_obtain: Enter your work email and Granite sends you to your company's sign-in page.
  name: SSO
  type: oauth2
slug: granite-md-authentication
source_filename: granite-md-authentication.yml
source_heading: Authentication Profile
source_url: https://granite.md/help/getting-started
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://granite.md/help/getting-started\nsources:\n- https://granite.md/help/getting-started\n- https://granite.md/help/getting-started/what-is-granite\n- https://granite.md/help/getting-started/create-account\n- https://granite.md/help/getting-started/sign-in-options\ndescription: Authentication methods described on Granite help pages.\nschemes:\n- type: http-basic\n  name: Email and password\n  evidence: Sign in with your email and password, with Google, with Apple, or with your company's single sign-on.\n  how_to_obtain: Sign up with your email and a password, or choose Continue with Google or Continue with Apple.\n- type: oauth2\n  name: Google\n  evidence: Continue with Google Use your Google account.\n  how_to_obtain: Continue with Google.\n- type: oauth2\n  name: Apple\n  evidence: Continue with Apple Use your Apple ID.\n  how_to_obtain: Continue with Apple.\n- type: oauth2\n\
  \  name: SSO\n  evidence: Continue with SSO For company workspaces that use Okta, Microsoft Entra ID, Google Workspace, or another identity provider.\n  how_to_obtain: Enter your work email and Granite sends you to your company's sign-in page.\ndocs: https://granite.md/help/getting-started\n"
source_yaml_url: https://artifacts.apis.io/granite-md/authentication/granite-md-authentication.yml
summary_line: 4 schemes
tags:
- Knowledge Base
- Artificial Intelligence
- Collaboration
- Security
- Encryption
---
