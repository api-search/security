---
api_key_in: []
api_specs:
- filename: reddit-ads-api-openapi.yml
  format: yaml
  label: Reddit Ads API
  slug: ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-ads-api-openapi.yml
- filename: reddit-account-api-openapi.yml
  format: yaml
  label: Reddit Account API
  slug: reddit-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-account-api-openapi.yml
- filename: reddit-accounts-api-openapi.yml
  format: yaml
  label: Reddit Accounts API
  slug: reddit-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-accounts-api-openapi.yml
- filename: reddit-ad-groups-api-openapi.yml
  format: yaml
  label: Reddit Ad Groups API
  slug: reddit-ad-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-ad-groups-api-openapi.yml
- filename: reddit-campaigns-api-openapi.yml
  format: yaml
  label: Reddit Campaigns API
  slug: reddit-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-campaigns-api-openapi.yml
- filename: reddit-conversions-api-openapi.yml
  format: yaml
  label: Reddit Conversions API
  slug: reddit-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-conversions-api-openapi.yml
- filename: reddit-custom-audiences-api-openapi.yml
  format: yaml
  label: Reddit Custom Audiences API
  slug: reddit-custom-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-custom-audiences-api-openapi.yml
- filename: reddit-flair-api-openapi.yml
  format: yaml
  label: Reddit Flair API
  slug: reddit-flair-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-flair-api-openapi.yml
- filename: reddit-funding-api-openapi.yml
  format: yaml
  label: Reddit Funding API
  slug: reddit-funding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-funding-api-openapi.yml
- filename: reddit-links-comments-api-openapi.yml
  format: yaml
  label: Reddit Links & Comments API
  slug: reddit-links-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-links-comments-api-openapi.yml
- filename: reddit-listings-api-openapi.yml
  format: yaml
  label: Reddit Listings API
  slug: reddit-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-listings-api-openapi.yml
- filename: reddit-messages-api-openapi.yml
  format: yaml
  label: Reddit Messages API
  slug: reddit-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-messages-api-openapi.yml
- filename: reddit-moderation-api-openapi.yml
  format: yaml
  label: Reddit Moderation API
  slug: reddit-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-moderation-api-openapi.yml
- filename: reddit-oembed-api-openapi.yml
  format: yaml
  label: Reddit oEmbed API
  slug: reddit-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-oembed-api-openapi.yml
- filename: reddit-reporting-api-openapi.yml
  format: yaml
  label: Reddit Reporting API
  slug: reddit-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-reporting-api-openapi.yml
- filename: reddit-search-api-openapi.yml
  format: yaml
  label: Reddit Search API
  slug: reddit-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-search-api-openapi.yml
- filename: reddit-subreddits-api-openapi.yml
  format: yaml
  label: Reddit Subreddits API
  slug: reddit-subreddits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-subreddits-api-openapi.yml
- filename: reddit-targeting-api-openapi.yml
  format: yaml
  label: Reddit Targeting API
  slug: reddit-targeting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-targeting-api-openapi.yml
- filename: reddit-users-api-openapi.yml
  format: yaml
  label: Reddit Users API
  slug: reddit-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-users-api-openapi.yml
- filename: reddit-wiki-api-openapi.yml
  format: yaml
  label: Reddit Wiki API
  slug: reddit-wiki-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-wiki-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Reddit Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Reddit secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Reddit
provider_slug: reddit
scheme_count: 1
schemes:
- description: Reddit Ads API uses OAuth 2.0 for authentication. Access tokens are obtained via the authorization code flow.
  flows:
  - authorizationUrl: https://www.reddit.com/api/v1/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://www.reddit.com/api/v1/access_token
  name: oauth2
  sources:
  - openapi/reddit-ads-api-openapi.yml
  - openapi/reddit-data-api-openapi.yml
  type: oauth2
slug: reddit-authentication
source_filename: reddit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reddit-ads-api-openapi.yml, openapi/reddit-data-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.reddit.com/api/v1/authorize\n    tokenUrl: https://www.reddit.com/api/v1/access_token\n    scopes: 1\n  description: Reddit Ads API uses OAuth 2.0 for authentication. Access tokens are obtained\n    via the authorization code flow.\n  sources:\n  - openapi/reddit-ads-api-openapi.yml\n  - openapi/reddit-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/authentication/reddit-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Advertising
- Communities
- Content
- Social-Media
- Social News
---
