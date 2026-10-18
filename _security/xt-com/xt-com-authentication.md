---
anonymous_access: false
api_key_in: []
api_specs:
- filename: xt-com-basic-error-controller-api-openapi.yml
  format: yaml
  label: XT.COM Basic Error Controller API
  slug: xt-com-basic-error-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xt-com/refs/heads/main/openapi/xt-com-basic-error-controller-api-openapi.yml
- filename: xt-com-default-api-openapi.yml
  format: yaml
  label: XT.COM 合约信息 API
  slug: xt-com-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xt-com/refs/heads/main/openapi/xt-com-default-api-openapi.yml
- filename: xt-com-listenkey-api-openapi.yml
  format: yaml
  label: XT.COM Listen Key API
  slug: xt-com-listenkey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xt-com/refs/heads/main/openapi/xt-com-listenkey-api-openapi.yml
- filename: xt-com-order-api-openapi.yml
  format: yaml
  label: XT.COM 合约聪明钱 Order API
  slug: xt-com-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xt-com/refs/heads/main/openapi/xt-com-order-api-openapi.yml
- filename: xt-com-symbol-controller-api-openapi.yml
  format: yaml
  label: XT.COM Symbol Controller API
  slug: xt-com-symbol-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xt-com/refs/heads/main/openapi/xt-com-symbol-controller-api-openapi.yml
- filename: xt-com-v2-api-openapi.yml
  format: yaml
  label: XT.COM 获取交易对配置信息(v2) API
  slug: xt-com-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xt-com/refs/heads/main/openapi/xt-com-v2-api-openapi.yml
- filename: xt-com-v3-api-openapi.yml
  format: yaml
  label: XT.COM 获取交易对配置信息(v3) API
  slug: xt-com-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xt-com/refs/heads/main/openapi/xt-com-v3-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Xt Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: XT.COM declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: XT.COM
provider_slug: xt-com
scheme_count: 1
schemes:
- description: API key (validate-appkey) plus an HMAC signature (validate-signature, default HmacSHA256; HmacMD5/SHA1/SHA224/SHA384/SHA512 supported) over the request, with a millisecond timestamp and a recvwindow (default 5 s, max 60 s). The published OpenAPI files declare no securitySchemes; this is read from the docs.
  headers:
  - validate-appkey
  - validate-timestamp
  - validate-signature
  - validate-recvwindow
  - validate-algorithms
  in: header
  name: XT HMAC signature headers
  type: apiKey
slug: xt-com-authentication
source_filename: xt-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: searched\nsource: https://github.com/XtApis/xt-api/blob/main/docs/futures/Access%20Description/signStatement.mdx\ndocs: https://doc.xt.com/futures\nschemes:\n- name: XT HMAC signature headers\n  type: apiKey\n  in: header\n  headers:\n  - validate-appkey\n  - validate-timestamp\n  - validate-signature\n  - validate-recvwindow\n  - validate-algorithms\n  description: API key (validate-appkey) plus an HMAC signature (validate-signature,\n    default HmacSHA256; HmacMD5/SHA1/SHA224/SHA384/SHA512 supported) over the request,\n    with a millisecond timestamp and a recvwindow (default 5 s, max 60 s). The published\n    OpenAPI files declare no securitySchemes; this is read from the docs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xt-com/refs/heads/main/authentication/xt-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Futures
- Market Data
- Blockchain
---
