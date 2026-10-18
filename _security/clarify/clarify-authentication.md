---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clarify-activities-api-openapi.yml
  format: yaml
  label: Clarify Activities API
  slug: clarify-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-activities-api-openapi.yml
- filename: clarify-campaigns-api-openapi.yml
  format: yaml
  label: Clarify Campaigns API
  slug: clarify-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-campaigns-api-openapi.yml
- filename: clarify-comments-api-openapi.yml
  format: yaml
  label: Clarify Comments API
  slug: clarify-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-comments-api-openapi.yml
- filename: clarify-invitations-api-openapi.yml
  format: yaml
  label: Clarify Invitations API
  slug: clarify-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-invitations-api-openapi.yml
- filename: clarify-layouts-api-openapi.yml
  format: yaml
  label: Clarify Layouts API
  slug: clarify-layouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-layouts-api-openapi.yml
- filename: clarify-listrows-api-openapi.yml
  format: yaml
  label: Clarify List Rows API
  slug: clarify-listrows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-listrows-api-openapi.yml
- filename: clarify-lists-api-openapi.yml
  format: yaml
  label: Clarify Lists API
  slug: clarify-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-lists-api-openapi.yml
- filename: clarify-meetingrecordings-api-openapi.yml
  format: yaml
  label: Clarify Meeting Recordings API
  slug: clarify-meetingrecordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-meetingrecordings-api-openapi.yml
- filename: clarify-objectaccess-api-openapi.yml
  format: yaml
  label: Clarify Object Access API
  slug: clarify-objectaccess-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-objectaccess-api-openapi.yml
- filename: clarify-recordaccess-api-openapi.yml
  format: yaml
  label: Clarify Record Access API
  slug: clarify-recordaccess-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-recordaccess-api-openapi.yml
- filename: clarify-recordattachments-api-openapi.yml
  format: yaml
  label: Clarify Record Attachments API
  slug: clarify-recordattachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-recordattachments-api-openapi.yml
- filename: clarify-recordrelationships-api-openapi.yml
  format: yaml
  label: Clarify Record Relationships API
  slug: clarify-recordrelationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-recordrelationships-api-openapi.yml
- filename: clarify-records-api-openapi.yml
  format: yaml
  label: Clarify Records API
  slug: clarify-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-records-api-openapi.yml
- filename: clarify-resources-api-openapi.yml
  format: yaml
  label: Clarify Resources API
  slug: clarify-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-resources-api-openapi.yml
- filename: clarify-schemas-api-openapi.yml
  format: yaml
  label: Clarify Schemas API
  slug: clarify-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-schemas-api-openapi.yml
- filename: clarify-users-api-openapi.yml
  format: yaml
  label: Clarify Users API
  slug: clarify-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-users-api-openapi.yml
- filename: clarify-workflows-api-openapi.yml
  format: yaml
  label: Clarify Workflows API
  slug: clarify-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-workflows-api-openapi.yml
- filename: clarify-workspacesettings-api-openapi.yml
  format: yaml
  label: Clarify Workspace Settings API
  slug: clarify-workspacesettings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-workspacesettings-api-openapi.yml
- filename: clarify-api-keys-api-openapi.yml
  format: yaml
  label: Clarify API Keys API
  slug: clarify-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-api-keys-api-openapi.yml
auth_types: []
description: Authentication methods for Clarify API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Clarify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clarify declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Clarify
provider_slug: clarify
scheme_count: 2
schemes:
- evidence: 'Send the key in the Authorization header using the api-key scheme, noting that this is not a Bearer token: Authorization: api-key YOUR_API_KEY'
  header: Authorization
  how_to_obtain: Create an API key in Settings → API Keys (personal or workspace).
  location: header
  name: api-key
  type: apiKey
- authorize_url: https://auth1.clarify.ai/oauth2/authorize
  evidence: Partner integrations authenticate with OAuth 2.0 and act on behalf of a Clarify user.
  header: Authorization
  how_to_obtain: 'Contact support@clarify.ai to register a client and receive a Client ID (and Client Secret for private apps). Use the Authorization Code flow (with PKCE for public apps) to obtain an access token, then send it as "Authorization: Bearer ACCESS_TOKEN".'
  location: header
  name: Clarify OAuth
  scopes:
  - openid
  - profile
  - email
  - offline_access
  type: oauth2
slug: clarify-authentication
source_filename: clarify-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.clarify.ai/docs/getting-started/authentication
source_yaml: "generated: '2026-10-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.clarify.ai/docs/getting-started/authentication\nsources:\n- https://developer.clarify.ai/docs/getting-started/authentication\n- https://developer.clarify.ai/docs/api-reference/apikeys/createApiKey\n- https://developer.clarify.ai/docs/api-reference/apikeys/deleteApiKey\n- https://developer.clarify.ai/docs/api-reference/apikeys/getApiKeys\ndescription: Authentication methods for Clarify API\nschemes:\n- type: apiKey\n  name: api-key\n  evidence: 'Send the key in the Authorization header using the api-key scheme, noting that this is not a Bearer token: Authorization: api-key\n    YOUR_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in Settings → API Keys (personal or workspace).\n- type: oauth2\n  name: Clarify OAuth\n  evidence: Partner integrations authenticate with OAuth 2.0 and act on behalf of a Clarify user.\n  location:\
  \ header\n  header: Authorization\n  authorize_url: https://auth1.clarify.ai/oauth2/authorize\n  scopes:\n  - openid\n  - profile\n  - email\n  - offline_access\n  how_to_obtain: 'Contact support@clarify.ai to register a client and receive a Client ID (and Client Secret for private apps). Use the Authorization\n    Code flow (with PKCE for public apps) to obtain an access token, then send it as \"Authorization: Bearer ACCESS_TOKEN\".'\ndocs: https://developer.clarify.ai/docs/getting-started/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/authentication/clarify-authentication.yml
summary_line: 2 schemes
tags:
- Company
- CRM
- Artificial Intelligence
- Automation
- Sales
---
