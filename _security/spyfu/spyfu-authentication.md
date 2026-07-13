---
api_key_in:
- header
- query
api_specs:
- filename: openapi.json
  format: json
  label: SpyFu API
  slug: spyfu-api
  spec_type: OpenAPI
  url: https://developer.spyfu.com/openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Spyfu Authentication
name_suffix: Authentication
oauth_flows: []
overview: SpyFu secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SpyFu
provider_slug: spyfu
scheme_count: 3
schemes:
- description: <a href="https://en.wikipedia.org/wiki/Basic_access_authentication#Client_side" target="_blank">Basic Authentication</a> is a standard that involves encoding your <code>SPYFU_API_ID:SECRET_KEY</code> into a Base64 string. Your <b>SpyFu API ID</b> and <b>Secret Key</b> can both be found under the <b><a href="https://www.spyfu.com/account/api" target="_blank">Account Settings -> API Usage</a></b> pa
  name: Basic_Authentication_Token
  scheme: basic
  sources:
  - openapi/spyfu-account-openapi.yml
  - openapi/spyfu-ad-history-openapi.yml
  - openapi/spyfu-competitors-openapi.yml
  - openapi/spyfu-domain-stats-openapi.yml
  - openapi/spyfu-keyword-related-openapi.yml
  - openapi/spyfu-kombat-openapi.yml
  - openapi/spyfu-ppc-keyword-openapi.yml
  - openapi/spyfu-ppc-research-serp-openapi.yml
  - openapi/spyfu-ranking-history-openapi.yml
  - openapi/spyfu-seo-research-serp-openapi.yml
  type: http
- description: An API key can be added as a query parameter. Your API key is listed as "Secret Key" found under the <b><a href="https://www.spyfu.com/account/api" target="_blank">Account Settings -> API Usage</a></b> page<br>For example, to authorize with the API key <code>AB12WXY</code><br><pre><code>/apis/example_api/GetExample?domain=spyfu.com<span class="token keyword">&api_key=AB12WXYZ</span></code></pre>
  in: query
  name: Query_Parameter_Token
  parameter: api_key
  sources:
  - openapi/spyfu-account-openapi.yml
  - openapi/spyfu-ad-history-openapi.yml
  - openapi/spyfu-competitors-openapi.yml
  - openapi/spyfu-domain-stats-openapi.yml
  - openapi/spyfu-keyword-related-openapi.yml
  - openapi/spyfu-kombat-openapi.yml
  - openapi/spyfu-ppc-keyword-openapi.yml
  - openapi/spyfu-ppc-research-serp-openapi.yml
  - openapi/spyfu-ranking-history-openapi.yml
  - openapi/spyfu-seo-research-serp-openapi.yml
  type: apiKey
- description: For even more security, each request can be individually authenticated with a timestamped <a href="https://en.wikipedia.org/wiki/HMAC" target="_blank"><b>HMAC</b></a> <em>(Hash Message Authentication Code)</em> signature. Composed of your secret key, a valid timestamp, the API request path, and all request parameters. <h3>Creating the signature:</h3><br>Combine the pieces that will be converted in
  in: header
  name: HMAC_Authentication_Header
  parameter: Authentication
  sources:
  - openapi/spyfu-account-openapi.yml
  - openapi/spyfu-ad-history-openapi.yml
  - openapi/spyfu-competitors-openapi.yml
  - openapi/spyfu-domain-stats-openapi.yml
  - openapi/spyfu-keyword-related-openapi.yml
  - openapi/spyfu-kombat-openapi.yml
  - openapi/spyfu-ppc-keyword-openapi.yml
  - openapi/spyfu-ppc-research-serp-openapi.yml
  - openapi/spyfu-ranking-history-openapi.yml
  - openapi/spyfu-seo-research-serp-openapi.yml
  type: apiKey
slug: spyfu-authentication
source_filename: spyfu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spyfu-account-openapi.yml, openapi/spyfu-ad-history-openapi.yml, openapi/spyfu-competitors-openapi.yml,\n  openapi/spyfu-domain-stats-openapi.yml, openapi/spyfu-keyword-related-openapi.yml, openapi/spyfu-kombat-openapi.yml,\n  openapi/spyfu-ppc-keyword-openapi.yml, openapi/spyfu-ppc-research-serp-openapi.yml, openapi/spyfu-ranking-history-openapi.yml,\n  openapi/spyfu-seo-research-serp-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: Basic_Authentication_Token\n  type: http\n  scheme: basic\n  description: <a href=\"https://en.wikipedia.org/wiki/Basic_access_authentication#Client_side\"\n    target=\"_blank\">Basic Authentication</a> is a standard that involves encoding your <code>SPYFU_API_ID:SECRET_KEY</code>\n    into a Base64 string. Your <b>SpyFu API ID</b> and <b>Secret Key</b> can both be found under\n    the <b><a href=\"https://www.spyfu.com/account/api\"\
  \ target=\"_blank\">Account Settings -> API\n    Usage</a></b> pa\n  sources:\n  - openapi/spyfu-account-openapi.yml\n  - openapi/spyfu-ad-history-openapi.yml\n  - openapi/spyfu-competitors-openapi.yml\n  - openapi/spyfu-domain-stats-openapi.yml\n  - openapi/spyfu-keyword-related-openapi.yml\n  - openapi/spyfu-kombat-openapi.yml\n  - openapi/spyfu-ppc-keyword-openapi.yml\n  - openapi/spyfu-ppc-research-serp-openapi.yml\n  - openapi/spyfu-ranking-history-openapi.yml\n  - openapi/spyfu-seo-research-serp-openapi.yml\n- name: Query_Parameter_Token\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: An API key can be added as a query parameter. Your API key is listed as \"Secret\n    Key\" found under the <b><a href=\"https://www.spyfu.com/account/api\" target=\"_blank\">Account\n    Settings -> API Usage</a></b> page<br>For example, to authorize with the API key <code>AB12WXY</code><br><pre><code>/apis/example_api/GetExample?domain=spyfu.com<span\n    class=\"token keyword\"\
  >&api_key=AB12WXYZ</span></code></pre>\n  sources:\n  - openapi/spyfu-account-openapi.yml\n  - openapi/spyfu-ad-history-openapi.yml\n  - openapi/spyfu-competitors-openapi.yml\n  - openapi/spyfu-domain-stats-openapi.yml\n  - openapi/spyfu-keyword-related-openapi.yml\n  - openapi/spyfu-kombat-openapi.yml\n  - openapi/spyfu-ppc-keyword-openapi.yml\n  - openapi/spyfu-ppc-research-serp-openapi.yml\n  - openapi/spyfu-ranking-history-openapi.yml\n  - openapi/spyfu-seo-research-serp-openapi.yml\n- name: HMAC_Authentication_Header\n  type: apiKey\n  in: header\n  parameter: Authentication\n  description: For even more security, each request can be individually authenticated with a\n    timestamped <a href=\"https://en.wikipedia.org/wiki/HMAC\" target=\"_blank\"><b>HMAC</b></a>\n    <em>(Hash Message Authentication Code)</em> signature. Composed of your secret key, a valid\n    timestamp, the API request path, and all request parameters. <h3>Creating the signature:</h3><br>Combine\n    the pieces\
  \ that will be converted in\n  sources:\n  - openapi/spyfu-account-openapi.yml\n  - openapi/spyfu-ad-history-openapi.yml\n  - openapi/spyfu-competitors-openapi.yml\n  - openapi/spyfu-domain-stats-openapi.yml\n  - openapi/spyfu-keyword-related-openapi.yml\n  - openapi/spyfu-kombat-openapi.yml\n  - openapi/spyfu-ppc-keyword-openapi.yml\n  - openapi/spyfu-ppc-research-serp-openapi.yml\n  - openapi/spyfu-ranking-history-openapi.yml\n  - openapi/spyfu-seo-research-serp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spyfu/refs/heads/main/authentication/spyfu-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- SEO
- PPC
- Competitive Intelligence
- Keyword Research
- Ad History
- Backlinks
- Domain Analytics
- SERP
---
