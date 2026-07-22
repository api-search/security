---
api_key_in:
- header
api_specs:
- filename: revolut-business-openapi.yaml
  format: yaml
  label: Revolut Business API
  slug: revolut-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revolut/refs/heads/main/openapi/revolut-business-openapi.yaml
- filename: revolut-merchant-openapi.yaml
  format: yaml
  label: Revolut Merchant API
  slug: revolut-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revolut/refs/heads/main/openapi/revolut-merchant-openapi.yaml
- filename: revolut-open-banking-openapi.yaml
  format: yaml
  label: Revolut Open Banking API
  slug: revolut-open-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revolut/refs/heads/main/openapi/revolut-open-banking-openapi.yaml
- filename: revolut-crypto-ramp-openapi.yaml
  format: yaml
  label: Revolut Crypto Ramp API
  slug: revolut-crypto-ramp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revolut/refs/heads/main/openapi/revolut-crypto-ramp-openapi.yaml
- filename: revolut-x-openapi.yaml
  format: yaml
  label: Revolut X API
  slug: revolut-x-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revolut/refs/heads/main/openapi/revolut-x-openapi.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Revolut Authentication
name_suffix: Authentication
oauth_flows: []
overview: Revolut secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Revolut
provider_slug: revolut
scheme_count: 5
schemes:
- description: "Each Business API request must contain an authorization header in the following format to make a call: `Bearer <your_access_token>`.\n\nThe access token will be obtained the first time you set up your application and has an expiration of 40 minutes. \nDuring setup, a `refresh_token` will also be obtained which allows to obtain a new `access_token`.\n\n:::danger\nNever share your client-assertion JWT (JS"
  name: AccessToken
  scheme: bearer
  sources:
  - openapi/revolut-business-openapi.yaml
  type: http
- description: "Each Crypto Ramp API request must contain an authorization header in the following format to make a call: `X-API-KEY: {your_API_key}`. \n\nBefore you start, make sure that you have the correct API key. For more information, see the **Get started** guides: [Integrate with Revolut Ramp -> 2. Get Partner keys](https://developer.revolut.com/docs/guides/crypto-ramp/get-started/integrate-with-revolut-ramp"
  in: header
  name: AccessToken
  parameter: X-API-KEY
  sources:
  - openapi/revolut-crypto-ramp-openapi.yaml
  type: apiKey
- description: 'Each Merchant API request must contain an authorization header in the following format:


    ```

    ''Authorization: Bearer <yourSecretApiKey>''

    ```


    To use this API, you need to generate API keys from your Revolut Business account. The Secret key is used in the authorization header for all server calls, while the Public key is provided with payment methods at checkout.


    :::info

    For detailed instructions o'
  in: header
  name: Api-Key
  parameter: Authorization
  sources:
  - openapi/revolut-merchant-openapi.yaml
  - openapi/revolut-open-banking-openapi.yaml
  type: apiKey
- description: 'Open Banking API Payment requests additionally require a JSON Web Signature (JWS) which needs to be added to the header of the request.

    The JWS signature must be obtained using the full content of the payload.'
  in: header
  name: JWS
  parameter: x-jws-signature
  sources:
  - openapi/revolut-open-banking-openapi.yaml
  type: apiKey
- description: "The [API key](https://developer.revolut.com/docs/api/revolut-x-crypto-exchange#api-key) obtained from the [Revolut X web app](https://exchange.revolut.com/).\nIt takes the form of a 64-character alphanumeric string, and must be provided with other authentication headers.\n\nA sample API key might look like this: \n```sh\nM1VKFtwB0M9C9QJO7goPlwrOytrJsSNE19txsmpsWIKz7xYu3f8aNucIyynAhYBy\n```\n\nEach API key"
  in: header
  name: ApiKey
  parameter: X-Revx-API-Key
  sources:
  - openapi/revolut-x-openapi.yaml
  type: apiKey
slug: revolut-authentication
source_filename: revolut-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/revolut-business-openapi.yaml, openapi/revolut-crypto-ramp-openapi.yaml, openapi/revolut-merchant-openapi.yaml,\n  openapi/revolut-open-banking-openapi.yaml, openapi/revolut-x-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: AccessToken\n  type: http\n  scheme: bearer\n  description: \"Each Business API request must contain an authorization header in the following\\\n    \\ format to make a call: `Bearer <your_access_token>`.\\n\\nThe access token will be obtained\\\n    \\ the first time you set up your application and has an expiration of 40 minutes. \\nDuring\\\n    \\ setup, a `refresh_token` will also be obtained which allows to obtain a new `access_token`.\\n\\\n    \\n:::danger\\nNever share your client-assertion JWT (JS\"\n  sources:\n  - openapi/revolut-business-openapi.yaml\n- name: AccessToken\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description:\
  \ \"Each Crypto Ramp API request must contain an authorization header in the following\\\n    \\ format to make a call: `X-API-KEY: {your_API_key}`. \\n\\nBefore you start, make sure that\\\n    \\ you have the correct API key. For more information, see the **Get started** guides: [Integrate\\\n    \\ with Revolut Ramp -> 2. Get Partner keys](https://developer.revolut.com/docs/guides/crypto-ramp/get-started/integrate-with-revolut-ramp\"\n  sources:\n  - openapi/revolut-crypto-ramp-openapi.yaml\n- name: Api-Key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Each Merchant API request must contain an authorization header in the following format:\n\n    ```\n    'Authorization: Bearer <yourSecretApiKey>'\n    ```\n\n    To use this API, you need to generate API keys from your Revolut Business account. The Secret key is used in the authorization header for all server calls, while the Public key is provided with payment methods at checkout.\n\n    :::info\n\
  \    For detailed instructions o\n  sources:\n  - openapi/revolut-merchant-openapi.yaml\n  - openapi/revolut-open-banking-openapi.yaml\n- name: JWS\n  type: apiKey\n  in: header\n  parameter: x-jws-signature\n  description: |-\n    Open Banking API Payment requests additionally require a JSON Web Signature (JWS) which needs to be added to the header of the request.\n    The JWS signature must be obtained using the full content of the payload.\n  sources:\n  - openapi/revolut-open-banking-openapi.yaml\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-Revx-API-Key\n  description: \"The [API key](https://developer.revolut.com/docs/api/revolut-x-crypto-exchange#api-key)\\\n    \\ obtained from the [Revolut X web app](https://exchange.revolut.com/).\\nIt takes the form\\\n    \\ of a 64-character alphanumeric string, and must be provided with other authentication\\\n    \\ headers.\\n\\nA sample API key might look like this: \\n```sh\\nM1VKFtwB0M9C9QJO7goPlwrOytrJsSNE19txsmpsWIKz7xYu3f8aNucIyynAhYBy\\\
  n\\\n    ```\\n\\nEach API key\"\n  sources:\n  - openapi/revolut-x-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revolut/refs/heads/main/authentication/revolut-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- Company
- Fintech
- Payments
- Banking
- Open Banking
- Merchant Acquiring
- Cryptocurrency
- Cards
---
