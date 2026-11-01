---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: 550Wai Cn Authentication
name_suffix: Authentication
oauth_flows: []
overview: 550wai-cn declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: 550wai-cn
provider_slug: 550wai-cn
scheme_count: 2
schemes:
- description: 用户编号（主账号）
  in: body
  name: userNo
  type: apiKey
- description: API 密钥，主密钥或子密钥
  in: body
  name: apiKey
  type: apiKey
slug: 550wai-cn-authentication
source_filename: 550wai-cn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://qzm.550wai.cn/api-open/#conventions\nschemes:\n  - type: apiKey\n    name: userNo\n    in: body\n    description: 用户编号（主账号）\n  - type: apiKey\n    name: apiKey\n    in: body\n    description: API 密钥，主密钥或子密钥\n"
source_yaml_url: https://artifacts.apis.io/550wai-cn/authentication/550wai-cn-authentication.yml
summary_line: 2 schemes
tags:
- AI
- VideoProcessing
- ImageProcessing
- WatermarkRemoval
- SubtitleRemoval
---
