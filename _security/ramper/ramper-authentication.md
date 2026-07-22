---
api_key_in:
- config
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Ramper Authentication
name_suffix: Authentication
oauth_flows:
- social-login
overview: Ramper secures its APIs with apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the social-login flow(s).
provider_name: Ramper
provider_slug: ramper
scheme_count: 3
schemes:
- description: App ID supplied to the SDK init() function.
  in: config
  name: RamperAppId
  sources:
  - docs
  type: apiKey
- description: App Secret used server-side to verify the user idToken.
  in: server
  name: RamperAppSecret
  sources:
  - docs
  type: apiKey
- description: End-user social OAuth login (Email/Google/Facebook/Apple/Twitter) that creates or unlocks a self-custody wallet and issues an idToken.
  flow: social-login
  name: RamperSocialLogin
  sources:
  - docs
  type: oauth2
slug: ramper-authentication
source_filename: ramper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.ramper.xyz/developer-guide/developer-dashboard + https://docs.ramper.xyz/embedded-wallet-sdk/quickstart/for-web-apps/version-1/sdk-specifications/initialization\ndocs: https://docs.ramper.xyz/developer-guide/developer-dashboard\nnotes: >-\n  Ramper is an SDK-first embedded wallet product with no public REST API, so this\n  auth profile is captured from the developer documentation rather than derived\n  from an OpenAPI spec. Two layers of authentication apply: (1) the DApp-to-Ramper\n  app credentials issued by the Developer Dashboard, and (2) the end-user social\n  login that mints a self-custody wallet.\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_in: [config]\n  oauth2_flows: [social-login]\napp_credentials:\n  - name: App ID\n    role: public client identifier passed to the SDK init() function; used to track user activity.\n    secret: false\n  - name: App Secret\n    role: server-side secret\
  \ used to verify the issued idToken and manage user sessions.\n    secret: true\n    warning: Never expose the App Secret in client-side code.\nend_user_auth:\n  model: social-login (OAuth) to non-custodial wallet\n  session_token: idToken (JWT verified server-side with the App Secret)\n  providers:\n    - Email\n    - Google\n    - Facebook\n    - Apple\n    - Twitter\n  self_custody: true\nschemes:\n  - name: RamperAppId\n    type: apiKey\n    in: config\n    description: App ID supplied to the SDK init() function.\n    sources: [docs]\n  - name: RamperAppSecret\n    type: apiKey\n    in: server\n    description: App Secret used server-side to verify the user idToken.\n    sources: [docs]\n  - name: RamperSocialLogin\n    type: oauth2\n    flow: social-login\n    description: End-user social OAuth login (Email/Google/Facebook/Apple/Twitter) that creates or unlocks a self-custody wallet and issues an idToken.\n    sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ramper/refs/heads/main/authentication/ramper-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 3 schemes
tags:
- Company
- Web3
- Wallet
- Embedded Wallet
- Blockchain
- Social Login
- Authentication
- SDK
- NFT
- Cryptocurrency
- DeFi
---
