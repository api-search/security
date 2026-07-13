---
api_key_in:
- header
api_specs:
- filename: acquia-cloud-openapi.yml
  format: yaml
  label: Acquia Cloud API
  slug: acquia-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-cloud-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Acquia Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Acquia secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Acquia
provider_slug: acquia
scheme_count: 2
schemes:
- description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.


    ### To generate a token:


    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.

    2. Click your user avatar in the upper right corner, and then click **Account Settings**.

    3. On the Profile page'
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://accounts.acquia.com/api/token
  name: Acquia_Cloud_API_Documentation_OAuth2
  sources:
  - openapi/acquia-cloud-account.yml
  - openapi/acquia-cloud-agreements.yml
  - openapi/acquia-cloud-application-performance-monitoring-services.yml
  - openapi/acquia-cloud-applications.yml
  - openapi/acquia-cloud-cloud-ide.yml
  - openapi/acquia-cloud-codebases.yml
  - openapi/acquia-cloud-current-system-health.yml
  - openapi/acquia-cloud-distributions.yml
  - openapi/acquia-cloud-email.yml
  - openapi/acquia-cloud-environments.yml
  - openapi/acquia-cloud-identity-providers.yml
  - openapi/acquia-cloud-invite.yml
  - openapi/acquia-cloud-messages.yml
  - openapi/acquia-cloud-notifications.yml
  - openapi/acquia-cloud-openapi-full.yml
  - openapi/acquia-cloud-options.yml
  - openapi/acquia-cloud-organizations.yml
  - openapi/acquia-cloud-private-networks.yml
  - openapi/acquia-cloud-subscriptions.yml
  - openapi/acquia-cloud-teams-and-permissions.yml
  type: oauth2
- description: Value for the Authorization header parameter.
  in: header
  name: Codebase_Service_JWT
  parameter: Authorization
  sources:
  - openapi/acquia-cloud-account.yml
  - openapi/acquia-cloud-agreements.yml
  - openapi/acquia-cloud-application-performance-monitoring-services.yml
  - openapi/acquia-cloud-applications.yml
  - openapi/acquia-cloud-cloud-ide.yml
  - openapi/acquia-cloud-codebases.yml
  - openapi/acquia-cloud-current-system-health.yml
  - openapi/acquia-cloud-distributions.yml
  - openapi/acquia-cloud-email.yml
  - openapi/acquia-cloud-environments.yml
  - openapi/acquia-cloud-identity-providers.yml
  - openapi/acquia-cloud-invite.yml
  - openapi/acquia-cloud-messages.yml
  - openapi/acquia-cloud-notifications.yml
  - openapi/acquia-cloud-openapi-full.yml
  - openapi/acquia-cloud-options.yml
  - openapi/acquia-cloud-organizations.yml
  - openapi/acquia-cloud-private-networks.yml
  - openapi/acquia-cloud-subscriptions.yml
  - openapi/acquia-cloud-teams-and-permissions.yml
  type: apiKey
slug: acquia-authentication
source_filename: acquia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/acquia-cloud-account.yml, openapi/acquia-cloud-agreements.yml, openapi/acquia-cloud-application-performance-monitoring-services.yml,\n  openapi/acquia-cloud-applications.yml, openapi/acquia-cloud-cloud-ide.yml, openapi/acquia-cloud-codebases.yml,\n  openapi/acquia-cloud-current-system-health.yml, openapi/acquia-cloud-distributions.yml, openapi/acquia-cloud-email.yml,\n  openapi/acquia-cloud-environments.yml, openapi/acquia-cloud-identity-providers.yml, openapi/acquia-cloud-invite.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n    scopes: 0\n  description: |-\n    All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on\
  \ your Acquia Profile page.\n\n    ### To generate a token:\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n    3. On the Profile page\n  sources:\n  - openapi/acquia-cloud-account.yml\n  - openapi/acquia-cloud-agreements.yml\n  - openapi/acquia-cloud-application-performance-monitoring-services.yml\n  - openapi/acquia-cloud-applications.yml\n  - openapi/acquia-cloud-cloud-ide.yml\n  - openapi/acquia-cloud-codebases.yml\n  - openapi/acquia-cloud-current-system-health.yml\n  - openapi/acquia-cloud-distributions.yml\n  - openapi/acquia-cloud-email.yml\n  - openapi/acquia-cloud-environments.yml\n  - openapi/acquia-cloud-identity-providers.yml\n  - openapi/acquia-cloud-invite.yml\n  - openapi/acquia-cloud-messages.yml\n  - openapi/acquia-cloud-notifications.yml\n  - openapi/acquia-cloud-openapi-full.yml\n  - openapi/acquia-cloud-options.yml\n\
  \  - openapi/acquia-cloud-organizations.yml\n  - openapi/acquia-cloud-private-networks.yml\n  - openapi/acquia-cloud-subscriptions.yml\n  - openapi/acquia-cloud-teams-and-permissions.yml\n- name: Codebase_Service_JWT\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Value for the Authorization header parameter.\n  sources:\n  - openapi/acquia-cloud-account.yml\n  - openapi/acquia-cloud-agreements.yml\n  - openapi/acquia-cloud-application-performance-monitoring-services.yml\n  - openapi/acquia-cloud-applications.yml\n  - openapi/acquia-cloud-cloud-ide.yml\n  - openapi/acquia-cloud-codebases.yml\n  - openapi/acquia-cloud-current-system-health.yml\n  - openapi/acquia-cloud-distributions.yml\n  - openapi/acquia-cloud-email.yml\n  - openapi/acquia-cloud-environments.yml\n  - openapi/acquia-cloud-identity-providers.yml\n  - openapi/acquia-cloud-invite.yml\n  - openapi/acquia-cloud-messages.yml\n  - openapi/acquia-cloud-notifications.yml\n  - openapi/acquia-cloud-openapi-full.yml\n\
  \  - openapi/acquia-cloud-options.yml\n  - openapi/acquia-cloud-organizations.yml\n  - openapi/acquia-cloud-private-networks.yml\n  - openapi/acquia-cloud-subscriptions.yml\n  - openapi/acquia-cloud-teams-and-permissions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/authentication/acquia-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Content
- Experience
---
