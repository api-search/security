---
api_key_in:
- header
- query
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Baidu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Baidu secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Baidu
provider_slug: baidu
scheme_count: 3
schemes:
- base_url: https://qianfan.baidubce.com/v2
  docs: https://intl.cloud.baidu.com/doc/qianfan/index.html
  format: API key prefixed bce-v3/ALTAK-..., created in the Baidu Intelligent Cloud console (Security Authentication > API Key)
  location: Authorization header
  name: qianfan-bearer
  openai_compatible: true
  product: Baidu AI Cloud Qianfan (LLM / MaaS)
  scheme: bearer
  type: http
- docs: https://intl.cloud.baidu.com/doc/Reference/s/Njwvz1wot
  location: Authorization header (BCE signing with Access Key + Secret Key)
  name: bce-ak-sk-signature
  product: Baidu Cloud (BCE) IAM signed requests / SDKs
  scheme: signature
  type: apiKey
- docs: https://lbsyun.baidu.com/faq/api?title=webapi/appendix
  in: query
  name: maps-ak
  optional_signature: SN (SHA-1 signature over request + SK) for server-side keys
  parameter: ak
  product: Baidu Maps Open Platform (LBS Web Service API)
  type: apiKey
slug: baidu-authentication
source_filename: baidu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://intl.cloud.baidu.com/doc/qianfan/index.html, https://lbsyun.baidu.com/faq/api?title=webapi\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header, query]\nnotes: >\n  Baidu has no single unified auth model — each product line documents its own scheme.\nschemes:\n  - name: qianfan-bearer\n    product: Baidu AI Cloud Qianfan (LLM / MaaS)\n    type: http\n    scheme: bearer\n    location: Authorization header\n    format: \"API key prefixed bce-v3/ALTAK-..., created in the Baidu Intelligent Cloud console (Security Authentication > API Key)\"\n    openai_compatible: true\n    base_url: https://qianfan.baidubce.com/v2\n    docs: https://intl.cloud.baidu.com/doc/qianfan/index.html\n  - name: bce-ak-sk-signature\n    product: Baidu Cloud (BCE) IAM signed requests / SDKs\n    type: apiKey\n    scheme: signature\n    location: Authorization header (BCE signing with Access Key + Secret Key)\n    docs: https://intl.cloud.baidu.com/doc/Reference/s/Njwvz1wot\n\
  \  - name: maps-ak\n    product: Baidu Maps Open Platform (LBS Web Service API)\n    type: apiKey\n    in: query\n    parameter: ak\n    optional_signature: SN (SHA-1 signature over request + SK) for server-side keys\n    docs: https://lbsyun.baidu.com/faq/api?title=webapi/appendix\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baidu/refs/heads/main/authentication/baidu-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Technology
- Artificial Intelligence
- Machine Learning
- LLM
- Maps
- Geolocation
- Cloud
- China
---
