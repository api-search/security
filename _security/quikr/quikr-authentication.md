---
api_key_in: []
api_specs:
- filename: quikr-app-api-openapi.yml
  format: yaml
  label: Quikr App API
  slug: quikr-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quikr/refs/heads/main/openapi/quikr-app-api-openapi.yml
- filename: quikr-platform-api-openapi.yml
  format: yaml
  label: Quikr Platform API
  slug: quikr-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quikr/refs/heads/main/openapi/quikr-platform-api-openapi.yml
- filename: quikr-public-api-openapi.yml
  format: yaml
  label: Quikr Public API
  slug: quikr-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quikr/refs/heads/main/openapi/quikr-public-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Quikr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quikr declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Quikr
provider_slug: quikr
scheme_count: 1
schemes:
- algorithm: HMAC-SHA1
  headers:
  - description: Application identifier issued to the approved partner app.
    name: X-Quikr-App-Id
  - description: Daily access token obtained via POST /app/auth/access_token; valid for one day, then must be regenerated.
    name: X-Quikr-Token-Id
  - description: HMAC-SHA1 signature of the request computed with the app secret.
    name: X-Quikr-Signature-v2
  id: quikr-signature-v2
  in: header
  standard: custom-hmac
  token_endpoint: https://api.quikr.com/app/auth/access_token
  token_lifetime: 1 day
  type: apiKey
slug: quikr-authentication
source_filename: quikr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.quikr.com/index.php/documentation\ndocs: https://developer.quikr.com/index.php/documentation\nname: Quikr Developer Platform Authentication\nsummary: >-\n  Quikr uses a custom HMAC-SHA1 request-signing scheme (not OAuth 2.0). Every\n  request carries an application id, a daily access token, and a computed\n  signature across three request headers. Access is invitation-only beta.\nschemes:\n- id: quikr-signature-v2\n  type: apiKey\n  in: header\n  standard: custom-hmac\n  algorithm: HMAC-SHA1\n  headers:\n  - name: X-Quikr-App-Id\n    description: Application identifier issued to the approved partner app.\n  - name: X-Quikr-Token-Id\n    description: >-\n      Daily access token obtained via POST /app/auth/access_token; valid for one\n      day, then must be regenerated.\n  - name: X-Quikr-Signature-v2\n    description: HMAC-SHA1 signature of the request computed with the app secret.\n  token_endpoint: https://api.quikr.com/app/auth/access_token\n\
  \  token_lifetime: 1 day\nhelper_libraries:\n- language: Java\n  name: QDP Java library\n  purpose: Generates the Quikr auth headers/signature.\n- language: PHP\n  name: QDP PHP library\n  purpose: Generates the Quikr auth headers/signature.\naccess_model: invitation-only-beta (request via dvlpr-support@quikr.com)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quikr/refs/heads/main/authentication/quikr-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Classifieds
- Marketplace
- Real Estate
- Automotive
- Jobs
- Ecommerce
- India
- Developer Platform
---
