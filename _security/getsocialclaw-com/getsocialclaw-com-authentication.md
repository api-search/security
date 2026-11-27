---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getsocialclaw-com-analytics-api-openapi.yml
  format: yaml
  label: SocialClaw Analytics API
  slug: getsocialclaw-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getsocialclaw-com/openapi/getsocialclaw-com-analytics-api-openapi.yml
- filename: getsocialclaw-com-assets-and-media-delivery-api-openapi.yml
  format: yaml
  label: SocialClaw Assets and Media Delivery API
  slug: getsocialclaw-com-assets-and-media-delivery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getsocialclaw-com/openapi/getsocialclaw-com-assets-and-media-delivery-api-openapi.yml
- filename: getsocialclaw-com-auth-billing-and-provider-callbacks-api-openapi.yml
  format: yaml
  label: SocialClaw Auth, Billing, and Provider Callbacks API
  slug: getsocialclaw-com-auth-billing-and-provider-callbacks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getsocialclaw-com/openapi/getsocialclaw-com-auth-billing-and-provider-callbacks-api-openapi.yml
- filename: getsocialclaw-com-browser-authentication-api-openapi.yml
  format: yaml
  label: SocialClaw Browser Authentication API
  slug: getsocialclaw-com-browser-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getsocialclaw-com/openapi/getsocialclaw-com-browser-authentication-api-openapi.yml
- filename: getsocialclaw-com-connections-and-accounts-api-openapi.yml
  format: yaml
  label: SocialClaw Connections and Accounts API
  slug: getsocialclaw-com-connections-and-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getsocialclaw-com/openapi/getsocialclaw-com-connections-and-accounts-api-openapi.yml
- filename: getsocialclaw-com-dashboard-browser-api-api-openapi.yml
  format: yaml
  label: SocialClaw Dashboard Browser API
  slug: getsocialclaw-com-dashboard-browser-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getsocialclaw-com/openapi/getsocialclaw-com-dashboard-browser-api-api-openapi.yml
- filename: getsocialclaw-com-publishing-runs-and-posts-api-openapi.yml
  format: yaml
  label: SocialClaw Publishing Runs and Posts API
  slug: getsocialclaw-com-publishing-runs-and-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getsocialclaw-com/openapi/getsocialclaw-com-publishing-runs-and-posts-api-openapi.yml
- filename: getsocialclaw-com-status-and-authentication-api-openapi.yml
  format: yaml
  label: SocialClaw Status and Authentication API
  slug: getsocialclaw-com-status-and-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getsocialclaw-com/openapi/getsocialclaw-com-status-and-authentication-api-openapi.yml
auth_types: []
description: Authentication uses an API key passed as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: SocialClaw Authentication
name_suffix: Authentication
oauth_flows: []
overview: SocialClaw declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: SocialClaw
provider_slug: getsocialclaw-com
scheme_count: 1
schemes:
- evidence: 'curl -sS https://getsocialclaw.com/v1/keys/validate \ -H "Authorization: Bearer $SOCIALCLAW_API_KEY"'
  header: Authorization
  how_to_obtain: Create a key in the dashboard
  location: header
  name: API Key
  type: apiKey
slug: getsocialclaw-com-authentication
source_filename: getsocialclaw-com-authentication.yml
source_heading: Authentication Profile
source_url: https://getsocialclaw.com/docs/quickstart
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://getsocialclaw.com/docs/quickstart\nsources:\n- https://getsocialclaw.com/docs/quickstart\ndescription: Authentication uses an API key passed as a Bearer token in the Authorization header.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'curl -sS https://getsocialclaw.com/v1/keys/validate \\ -H \"Authorization: Bearer $SOCIALCLAW_API_KEY\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the dashboard\ndocs: https://getsocialclaw.com/docs/quickstart\n"
source_yaml_url: https://artifacts.apis.io/getsocialclaw-com/authentication/getsocialclaw-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Social Media
- AI Agents
- Automation
- Scheduling
---
