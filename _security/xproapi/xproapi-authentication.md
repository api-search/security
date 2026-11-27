---
anonymous_access: false
api_key_in: []
api_specs:
- filename: xproapi-default-api-openapi.yml
  format: yaml
  label: Xproapi Default API
  slug: xproapi-default-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xproapi/openapi/xproapi-default-api-openapi.yml
- filename: xproapi-follow-followings-api-openapi.yml
  format: yaml
  label: Xproapi Follow, Followings API
  slug: xproapi-follow-followings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xproapi/openapi/xproapi-follow-followings-api-openapi.yml
- filename: xproapi-tweet-activity-api-openapi.yml
  format: yaml
  label: Xproapi Tweet Activity API
  slug: xproapi-tweet-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xproapi/openapi/xproapi-tweet-activity-api-openapi.yml
- filename: xproapi-tweets-api-openapi.yml
  format: yaml
  label: Xproapi Tweets API
  slug: xproapi-tweets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xproapi/openapi/xproapi-tweets-api-openapi.yml
- filename: xproapi-users-api-openapi.yml
  format: yaml
  label: Xproapi Users API
  slug: xproapi-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xproapi/openapi/xproapi-users-api-openapi.yml
- filename: xproapi-followers-api-openapi.yml
  format: yaml
  label: Xproapi Followers API
  slug: xproapi-followers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xproapi/openapi/xproapi-followers-api-openapi.yml
- filename: xproapi-following-api-openapi.yml
  format: yaml
  label: Xproapi Following API
  slug: xproapi-following-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xproapi/openapi/xproapi-following-api-openapi.yml
- filename: xproapi-mentions-api-openapi.yml
  format: yaml
  label: Xproapi Mentions API
  slug: xproapi-mentions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xproapi/openapi/xproapi-mentions-api-openapi.yml
auth_types: []
description: API uses a simple API key sent in the X-API-Key request header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Xproapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Xproapi declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Xproapi
provider_slug: xproapi
scheme_count: 1
schemes:
- evidence: Put the key in the X-API-Key request header.
  header: X-API-Key
  how_to_obtain: Create an API key in the Xproapi panel after confirming your email; the key starts with xp_ and is shown once after creation.
  location: header
  name: X-API-Key
  type: apiKey
slug: xproapi-authentication
source_filename: xproapi-authentication.yml
source_heading: Authentication Profile
source_url: https://xproapi.com/docs/guides/authentication/
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://xproapi.com/docs/guides/authentication/\nsources:\n- https://xproapi.com/docs/guides/authentication/\n- https://xproapi.com/register/\n- https://xproapi.com/login/\n- https://xproapi.com/docs/guides/authentication/\ndescription: API uses a simple API key sent in the X-API-Key request header.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: Put the key in the X-API-Key request header.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create an API key in the Xproapi panel after confirming your email; the key starts with xp_ and is shown once after creation.\nnote: No OAuth2, HTTP Bearer, or other authentication methods are documented on the provided pages.\ndocs: https://xproapi.com/docs/guides/authentication/\n"
source_yaml_url: https://artifacts.apis.io/xproapi/authentication/xproapi-authentication.yml
summary_line: 1 scheme
tags:
- Company
- X
- Social
- Monitoring
- Data
---
