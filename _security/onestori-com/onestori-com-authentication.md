---
anonymous_access: false
api_key_in: []
api_specs:
- filename: onestori-com-ai-api-openapi.yml
  format: yaml
  label: Stori AI API
  slug: onestori-com-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onestori-com/openapi/onestori-com-ai-api-openapi.yml
- filename: onestori-com-billing-api-openapi.yml
  format: yaml
  label: Stori Billing API
  slug: onestori-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onestori-com/openapi/onestori-com-billing-api-openapi.yml
- filename: onestori-com-email-api-openapi.yml
  format: yaml
  label: Stori Email API
  slug: onestori-com-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onestori-com/openapi/onestori-com-email-api-openapi.yml
- filename: onestori-com-jobs-api-openapi.yml
  format: yaml
  label: Stori Jobs API
  slug: onestori-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onestori-com/openapi/onestori-com-jobs-api-openapi.yml
- filename: onestori-com-partner-api-v1-api-openapi.yml
  format: yaml
  label: Stori Partner API v1 API
  slug: onestori-com-partner-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onestori-com/openapi/onestori-com-partner-api-v1-api-openapi.yml
- filename: onestori-com-profile-api-openapi.yml
  format: yaml
  label: Stori Profile API
  slug: onestori-com-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onestori-com/openapi/onestori-com-profile-api-openapi.yml
- filename: onestori-com-recruiter-api-openapi.yml
  format: yaml
  label: Stori Recruiter API
  slug: onestori-com-recruiter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onestori-com/openapi/onestori-com-recruiter-api-openapi.yml
- filename: onestori-com-traits-api-openapi.yml
  format: yaml
  label: Stori Traits API
  slug: onestori-com-traits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onestori-com/openapi/onestori-com-traits-api-openapi.yml
- filename: onestori-com-video-api-openapi.yml
  format: yaml
  label: Stori Video API
  slug: onestori-com-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onestori-com/openapi/onestori-com-video-api-openapi.yml
- filename: onestori-com-webhooks-api-openapi.yml
  format: yaml
  label: Stori Webhooks API
  slug: onestori-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onestori-com/openapi/onestori-com-webhooks-api-openapi.yml
auth_types: []
description: OAuth 2.0 authentication as published in the Stori OAuth metadata document.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Stori Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stori declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Stori
provider_slug: onestori-com
scheme_count: 1
schemes:
- authorize_url: https://www.onestori.com/oauth/authorize
  evidence: '"authorization_endpoint":"https://www.onestori.com/oauth/authorize"'
  flows:
  - authorization_code
  how_to_obtain: Register the client via the registration_endpoint (https://www.onestori.com/api/oauth/register) to receive client credentials.
  name: OAuth 2.0
  scopes:
  - read:jobs
  - read:candidates
  - read:credits
  - read:analytics
  - read:outreach
  - read:settings
  - write:candidates
  - write:jobs
  - write:pipeline
  - write:interviews
  - write:offers
  - write:outreach
  - write:settings
  - source:candidates
  - source:unlock
  - me:read:profile
  - me:read:stori
  - me:read:visibility
  - me:read:jobs
  - me:read:outreach
  - me:read:offers
  - me:read:account
  - me:write:profile
  - me:write:visibility
  - me:write:jobs
  - me:write:outreach
  - me:write:account
  - me:apply:jobs
  - me:source:contacts
  - me:source:unlock
  type: oauth2
slug: onestori-com-authentication
source_filename: onestori-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.onestori.com/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.onestori.com/.well-known/oauth-authorization-server\nsources:\n- https://www.onestori.com/.well-known/oauth-authorization-server\n- https://www.onestori.com/docs/clients/setup\ndescription: OAuth 2.0 authentication as published in the Stori OAuth metadata document.\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: '\"authorization_endpoint\":\"https://www.onestori.com/oauth/authorize\"'\n  flows:\n  - authorization_code\n  authorize_url: https://www.onestori.com/oauth/authorize\n  scopes:\n  - read:jobs\n  - read:candidates\n  - read:credits\n  - read:analytics\n  - read:outreach\n  - read:settings\n  - write:candidates\n  - write:jobs\n  - write:pipeline\n  - write:interviews\n  - write:offers\n  - write:outreach\n  - write:settings\n  - source:candidates\n  - source:unlock\n  - me:read:profile\n  - me:read:stori\n  - me:read:visibility\n  - me:read:jobs\n \
  \ - me:read:outreach\n  - me:read:offers\n  - me:read:account\n  - me:write:profile\n  - me:write:visibility\n  - me:write:jobs\n  - me:write:outreach\n  - me:write:account\n  - me:apply:jobs\n  - me:source:contacts\n  - me:source:unlock\n  how_to_obtain: Register the client via the registration_endpoint (https://www.onestori.com/api/oauth/register) to receive client credentials.\ndocs: https://www.onestori.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/onestori-com/authentication/onestori-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Hiring
- Artificial Intelligence
- Candidate Intelligence
- Recruiting
---
