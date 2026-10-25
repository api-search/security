---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bluescope Authentication
name_suffix: Authentication
oauth_flows: []
overview: BlueScope declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: BlueScope
provider_slug: bluescope
scheme_count: 2
schemes:
- credentials_issued:
  - client_id
  - client_secret
  - resource
  description: All Bluescope apis require an authorisation bearer token to ensure that you have the required roles to execute the api. This uses Microsoft's Oauth2.0 bearer token retrieval api.
  flow: clientCredentials
  format: Bearer
  header: Authorization
  in: header
  name: azureAdOAuth2
  onboarding: Email IntegrationSupport@bluescope.com with Organisation Name and Buyer Identifiers; Integration Support returns client_id, client_secret and resource.
  postman_collection: https://developer.apiaut.bluescope.com/content/OAuth2.0.postman_collection.json
  source: https://developer.apiaut.bluescope.com/GettingStartedPage_Authentication
  token_url: https://login.microsoftonline.com/bluescopeltd.onmicrosoft.com/oauth2/token
  type: oauth2
- alternate_query_parameter: subscription-key
  description: Bluecope apis requires you to provide a subscription key in the header for every HTTP request.
  header: Ocp-Apim-Subscription-Key
  in: header
  name: apimSubscriptionKey
  onboarding: Log in to the portal and subscribe to a Product; all subscriptions will remain inactive until it has been approved by the admin. Approved subscriptions show a primary and a secondary key.
  source: https://developer.apiaut.bluescope.com/GettingStartedPage_SubscriptionKeys
  type: apiKey
slug: bluescope-authentication
source_filename: bluescope-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: searched\nsource: https://developer.apiaut.bluescope.com/GettingStartedPage_Authentication\ndocs: https://developer.apiaut.bluescope.com/GettingStartedPage_Authentication\nname: BlueScope authentication\nnote: No OpenAPI is held (API definitions are visible only to signed-in, approved subscribers), so this profile is read from the Developer Centre Getting Started pages. The token endpoint was not called.\nschemes:\n- name: azureAdOAuth2\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://login.microsoftonline.com/bluescopeltd.onmicrosoft.com/oauth2/token\n  in: header\n  header: Authorization\n  format: Bearer\n  description: \"All Bluescope apis require an authorisation bearer token to ensure that you have the required roles to execute the api. This uses Microsoft's Oauth2.0 bearer token retrieval api.\"\n  onboarding: \"Email IntegrationSupport@bluescope.com with Organisation Name and Buyer Identifiers; Integration Support returns\
  \ client_id, client_secret and resource.\"\n  credentials_issued: [client_id, client_secret, resource]\n  postman_collection: https://developer.apiaut.bluescope.com/content/OAuth2.0.postman_collection.json\n  source: https://developer.apiaut.bluescope.com/GettingStartedPage_Authentication\n- name: apimSubscriptionKey\n  type: apiKey\n  in: header\n  header: Ocp-Apim-Subscription-Key\n  alternate_query_parameter: subscription-key\n  description: \"Bluecope apis requires you to provide a subscription key in the header for every HTTP request.\"\n  onboarding: \"Log in to the portal and subscribe to a Product; all subscriptions will remain inactive until it has been approved by the admin. Approved subscriptions show a primary and a secondary key.\"\n  source: https://developer.apiaut.bluescope.com/GettingStartedPage_SubscriptionKeys\ncombined: Both are required on BlueScope API calls (bearer token plus subscription key); the Microsoft token call itself needs no subscription key.\nportal_sign_in:\n\
  \  methods: [Basic (username and password), Azure Active Directory guest account]\n  source: https://developer.apiaut.bluescope.com/GettingStartedPage_SignupAndLogin\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluescope/refs/heads/main/authentication/bluescope-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Steel
- Manufacturing
- Building Materials
- Construction
- Australia
- ASX
---
