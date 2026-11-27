---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openanthropic-com-openapi-generated.yml
  format: yaml
  label: OpenAnthropic API
  slug: openanthropic-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openanthropic-com/openapi/_ae-authored/openanthropic-com-openapi-generated.yml
auth_types: []
description: Authentication methods for the Claude API
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: OpenAnthropic Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenAnthropic declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: OpenAnthropic
provider_slug: openanthropic-com
scheme_count: 4
schemes:
- evidence: API keys are static secrets that you generate in the Claude Console and send on every request as a bearer token in the `Authorization` header.
  header: Authorization
  how_to_obtain: Generate a key in the Claude Console under Settings → API keys.
  location: header
  name: API key
  type: http-bearer
- evidence: Short-lived bearer token exchanged from your identity provider’s identity token
  header: Authorization
  how_to_obtain: Exchange an identity provider token for a short‑lived bearer token via Workload Identity Federation as described in the Claude documentation.
  location: header
  name: Workload Identity Federation (WIF)
  type: http-bearer
- evidence: Short-lived access token issued to a genuine, attested installation of your registered iOS or macOS app
  header: Authorization
  how_to_obtain: Obtain an access token through the App Attest flow on iOS/macOS as described in the Claude documentation.
  location: header
  name: App Attest
  type: http-bearer
- evidence: Claude Platform OAuth uses the OAuth 2.0 authorization code flow with PKCE, with Anthropic as the authorization server.
  how_to_obtain: Create an OAuth app in the Claude Console and follow the authorization code flow with PKCE.
  name: Claude Platform OAuth
  type: oauth2
slug: openanthropic-com-authentication
source_filename: openanthropic-com-authentication.yml
source_heading: Authentication Profile
source_url: https://platform.claude.com/docs/en/manage-claude/authentication.md
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://platform.claude.com/docs/en/manage-claude/authentication.md\nsources:\n- https://platform.claude.com/docs/en/manage-claude/authentication.md\n- https://platform.claude.com/docs/en/get-api-key.md\n- https://platform.claude.com/docs/en/manage-claude/oauth-apps/overview.md\n- https://platform.claude.com/docs/en/manage-claude/oauth-apps/app-review.md\ndescription: Authentication methods for the Claude API\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: API keys are static secrets that you generate in the Claude Console and send on every request as a bearer token in the `Authorization`\n    header.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a key in the Claude Console under Settings → API keys.\n- type: http-bearer\n  name: Workload Identity Federation (WIF)\n  evidence: Short-lived bearer token exchanged from your identity provider’s\
  \ identity token\n  location: header\n  header: Authorization\n  how_to_obtain: Exchange an identity provider token for a short‑lived bearer token via Workload Identity Federation as described in the Claude\n    documentation.\n- type: http-bearer\n  name: App Attest\n  evidence: Short-lived access token issued to a genuine, attested installation of your registered iOS or macOS app\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain an access token through the App Attest flow on iOS/macOS as described in the Claude documentation.\n- type: oauth2\n  name: Claude Platform OAuth\n  evidence: Claude Platform OAuth uses the OAuth 2.0 authorization code flow with PKCE, with Anthropic as the authorization server.\n  how_to_obtain: Create an OAuth app in the Claude Console and follow the authorization code flow with PKCE.\ndocs: https://platform.claude.com/docs/en/manage-claude/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/openanthropic-com/authentication/openanthropic-com-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Artificial Intelligence
- Machine Learning
- LLM
- Safety
---
