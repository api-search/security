---
api_key_in: []
api_specs:
- filename: facebook-lead-ads-bulk-leads-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Bulk Leads API
  slug: facebook-lead-ads-bulk-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-bulk-leads-api-openapi.yml
- filename: facebook-lead-ads-leadgen-forms-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Leadgen Forms API
  slug: facebook-lead-ads-leadgen-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-leadgen-forms-api-openapi.yml
- filename: facebook-lead-ads-leads-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Leads API
  slug: facebook-lead-ads-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-leads-api-openapi.yml
- filename: facebook-lead-ads-meta-marketing-api-lead-ads-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Meta Marketing API Lead Ads API
  slug: facebook-lead-ads-meta-marketing-api-lead-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-meta-marketing-api-lead-ads-api-openapi.yml
- filename: facebook-lead-ads-subscribed-apps-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Subscribed Apps API
  slug: facebook-lead-ads-subscribed-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-subscribed-apps-api-openapi.yml
- filename: facebook-lead-ads-subscriptions-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Subscriptions API
  slug: facebook-lead-ads-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-subscriptions-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Facebook Lead Ads Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Facebook Lead Ads secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Facebook Lead Ads
provider_slug: facebook-lead-ads
scheme_count: 1
schemes:
- description: 'Page access token obtained via Facebook Login / Meta Business

    Login with leads_retrieval, pages_show_list, and

    pages_manage_ads permissions.'
  flows:
  - authorizationUrl: https://www.facebook.com/v22.0/dialog/oauth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://graph.facebook.com/v22.0/oauth/access_token
  name: PageAccessToken
  sources:
  - openapi/facebook-lead-ads-openapi.yml
  type: oauth2
slug: facebook-lead-ads-authentication
source_filename: facebook-lead-ads-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/facebook-lead-ads-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: PageAccessToken\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.facebook.com/v22.0/dialog/oauth\n    tokenUrl: https://graph.facebook.com/v22.0/oauth/access_token\n    scopes: 3\n  description: |-\n    Page access token obtained via Facebook Login / Meta Business\n    Login with leads_retrieval, pages_show_list, and\n    pages_manage_ads permissions.\n  sources:\n  - openapi/facebook-lead-ads-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/authentication/facebook-lead-ads-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Advertising
- Lead Generation
- Lead Ads
- Marketing API
- Facebook
- Instagram
- Meta
- Webhooks
---
