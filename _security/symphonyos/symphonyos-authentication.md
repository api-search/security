---
anonymous_access: false
api_key_in: []
api_specs:
- filename: symphonyos-openapi-generated.yml
  format: yaml
  label: SymphonyOS API
  slug: symphonyos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphonyos/refs/heads/main/openapi/_ae-authored/symphonyos-openapi-generated.yml
auth_types: []
description: Authentication schemes for SymphonyOS APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Symphonyos Authentication
name_suffix: Authentication
oauth_flows: []
overview: SymphonyOS declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: SymphonyOS
provider_slug: symphonyos
scheme_count: 2
schemes:
- evidence: 'All requests to the Ads API must include the following headers for authentication and security:'
  header: x-api-key
  how_to_obtain: Apply for partnership at https://www.symphonyos.co/partnerships; the team will provision an API key.
  location: header
  name: ApiKeyAuth
  type: apiKey
- evidence: If you intend to provide the API to your users directly, it is recommended to also send an `x-brand-id` header alongside your requests.
  header: x-brand-id
  how_to_obtain: Create a brand by either logging the user in with Facebook or calling the meta connect brand endpoint as described in the documentation.
  location: header
  name: BrandUserReference
  type: apiKey
slug: symphonyos-authentication
source_filename: symphonyos-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.symphonyos.co/docs/get-an-api-key.md
source_yaml: "generated: '2026-10-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.symphonyos.co/docs/get-an-api-key.md\nsources:\n- https://docs.symphonyos.co/docs/get-an-api-key.md\n- https://docs.symphonyos.co/docs/authentication.md\n- https://docs.symphonyos.co/reference/facebook-connect-brand-meta.md\n- https://docs.symphonyos.co/reference/facebook-connect-brand-meta-1.md\ndescription: Authentication schemes for SymphonyOS APIs\nschemes:\n- type: apiKey\n  name: ApiKeyAuth\n  evidence: 'All requests to the Ads API must include the following headers for authentication and security:'\n  location: header\n  header: x-api-key\n  how_to_obtain: Apply for partnership at https://www.symphonyos.co/partnerships; the team will provision an API key.\n- type: apiKey\n  name: BrandUserReference\n  evidence: If you intend to provide the API to your users directly, it is recommended to also send an `x-brand-id` header alongside your requests.\n  location: header\n\
  \  header: x-brand-id\n  how_to_obtain: Create a brand by either logging the user in with Facebook or calling the meta connect brand endpoint as described in the documentation.\nnote: No OAuth2, HTTP Bearer, HTTP Basic, JWT, HMAC, or mTLS schemes are documented.\ndocs: https://docs.symphonyos.co/docs/get-an-api-key.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/symphonyos/refs/heads/main/authentication/symphonyos-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Music
- Platform
- Agents
---
