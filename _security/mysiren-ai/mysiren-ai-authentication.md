---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mysiren-ai-account-webhooks-api-openapi.yml
  format: yaml
  label: Siren Account Webhooks API
  slug: mysiren-ai-account-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mysiren-ai/openapi/mysiren-ai-account-webhooks-api-openapi.yml
- filename: mysiren-ai-health-api-openapi.yml
  format: yaml
  label: Siren Health API
  slug: mysiren-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mysiren-ai/openapi/mysiren-ai-health-api-openapi.yml
- filename: mysiren-ai-programmatic-ads-api-openapi.yml
  format: yaml
  label: Siren Programmatic Ads API
  slug: mysiren-ai-programmatic-ads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mysiren-ai/openapi/mysiren-ai-programmatic-ads-api-openapi.yml
- filename: mysiren-ai-programmatic-api-openapi.yml
  format: yaml
  label: Siren Programmatic API
  slug: mysiren-ai-programmatic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mysiren-ai/openapi/mysiren-ai-programmatic-api-openapi.yml
- filename: mysiren-ai-programmatic-help-api-openapi.yml
  format: yaml
  label: Siren Programmatic Help API
  slug: mysiren-ai-programmatic-help-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mysiren-ai/openapi/mysiren-ai-programmatic-help-api-openapi.yml
- filename: mysiren-ai-studio-api-openapi.yml
  format: yaml
  label: Siren Studio API
  slug: mysiren-ai-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mysiren-ai/openapi/mysiren-ai-studio-api-openapi.yml
- filename: mysiren-ai-studio-custom-templates-api-openapi.yml
  format: yaml
  label: Siren Studio Custom Templates API
  slug: mysiren-ai-studio-custom-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mysiren-ai/openapi/mysiren-ai-studio-custom-templates-api-openapi.yml
- filename: mysiren-ai-studio-sessions-api-openapi.yml
  format: yaml
  label: Siren Studio Sessions API
  slug: mysiren-ai-studio-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mysiren-ai/openapi/mysiren-ai-studio-sessions-api-openapi.yml
auth_types: []
description: Siren uses OAuth 2.0 to connect social media accounts. Users click the OAuth button on the Connected Accounts page, are sent to the platform’s authorization screen, grant specific scopes, and Siren receives an OAuth token which it stores encrypted.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Siren Authentication
name_suffix: Authentication
oauth_flows: []
overview: Siren declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Siren
provider_slug: mysiren-ai
scheme_count: 1
schemes:
- evidence: Clicking Connect sends you to the platform's own authorization screen. You grant Siren specific scopes.
  flows:
  - authorization_code
  how_to_obtain: User clicks the OAuth button on Settings → Connected Accounts, authorizes on the platform’s screen, and Siren receives and stores the token.
  name: Platform OAuth
  scopes:
  - tweet.write
  - tweet.read
  - users.read
  - openid
  - profile
  - w_member_social
  - r_organization_social
  - w_organization_social
  - instagram_basic
  - instagram_content_publish
  - youtube.upload
  - user.info.basic
  - user.info.profile
  - video.publish
  - video.list
  type: oauth2
slug: mysiren-ai-authentication
source_filename: mysiren-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://mysiren.ai/docs/oauth-dispatch
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mysiren.ai/docs/oauth-dispatch\nsources:\n- https://mysiren.ai/docs/oauth-dispatch\n- https://mysiren.ai/docs/connect-first-channel\n- https://mysiren.ai/docs/getting-started\ndescription: Siren uses OAuth 2.0 to connect social media accounts. Users click the OAuth button on the Connected Accounts page, are sent to the\n  platform’s authorization screen, grant specific scopes, and Siren receives an OAuth token which it stores encrypted.\nschemes:\n- type: oauth2\n  name: Platform OAuth\n  evidence: Clicking Connect sends you to the platform's own authorization screen. You grant Siren specific scopes.\n  flows:\n  - authorization_code\n  scopes:\n  - tweet.write\n  - tweet.read\n  - users.read\n  - openid\n  - profile\n  - w_member_social\n  - r_organization_social\n  - w_organization_social\n  - instagram_basic\n  - instagram_content_publish\n  - youtube.upload\n  - user.info.basic\n\
  \  - user.info.profile\n  - video.publish\n  - video.list\n  how_to_obtain: User clicks the OAuth button on Settings → Connected Accounts, authorizes on the platform’s screen, and Siren receives and stores\n    the token.\ndocs: https://mysiren.ai/docs/oauth-dispatch\n"
source_yaml_url: https://artifacts.apis.io/mysiren-ai/authentication/mysiren-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Marketing
- Video
- Advertising
- Software-as-a-Service
---
