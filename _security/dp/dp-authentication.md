---
api_key_in: []
api_specs:
- filename: dp-ai-bohrium-mentor-api-openapi.yml
  format: yaml
  label: DP Technology (Bohrium) AI 科学小导师 (bohrium-mentor) API
  slug: dp-ai-bohrium-mentor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dp/refs/heads/main/openapi/dp-ai-bohrium-mentor-api-openapi.yml
- filename: dp-bohrium-dataset-api-openapi.yml
  format: yaml
  label: DP Technology (Bohrium) 数据集 (bohrium-dataset) API
  slug: dp-bohrium-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dp/refs/heads/main/openapi/dp-bohrium-dataset-api-openapi.yml
- filename: dp-bohrium-file-api-openapi.yml
  format: yaml
  label: DP Technology (Bohrium) 文件盘 (bohrium-file) API
  slug: dp-bohrium-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dp/refs/heads/main/openapi/dp-bohrium-file-api-openapi.yml
- filename: dp-bohrium-image-api-openapi.yml
  format: yaml
  label: DP Technology (Bohrium) 容器镜像 (bohrium-image) API
  slug: dp-bohrium-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dp/refs/heads/main/openapi/dp-bohrium-image-api-openapi.yml
- filename: dp-bohrium-job-api-openapi.yml
  format: yaml
  label: DP Technology (Bohrium) 计算任务 (bohrium-job) API
  slug: dp-bohrium-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dp/refs/heads/main/openapi/dp-bohrium-job-api-openapi.yml
- filename: dp-bohrium-knowledge-base-api-openapi.yml
  format: yaml
  label: DP Technology (Bohrium) 知识库 (bohrium-knowledge-base) API
  slug: dp-bohrium-knowledge-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dp/refs/heads/main/openapi/dp-bohrium-knowledge-base-api-openapi.yml
- filename: dp-bohrium-lkm-api-openapi.yml
  format: yaml
  label: DP Technology (Bohrium) 大知识模型 (bohrium-lkm) API
  slug: dp-bohrium-lkm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dp/refs/heads/main/openapi/dp-bohrium-lkm-api-openapi.yml
- filename: dp-bohrium-node-api-openapi.yml
  format: yaml
  label: DP Technology (Bohrium) 开发节点 (bohrium-node) API
  slug: dp-bohrium-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dp/refs/heads/main/openapi/dp-bohrium-node-api-openapi.yml
- filename: dp-bohrium-paper-search-api-openapi.yml
  format: yaml
  label: DP Technology (Bohrium) 论文与专利搜索 (bohrium-paper-search) API
  slug: dp-bohrium-paper-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dp/refs/heads/main/openapi/dp-bohrium-paper-search-api-openapi.yml
- filename: dp-bohrium-project-api-openapi.yml
  format: yaml
  label: DP Technology (Bohrium) 项目管理 (bohrium-project) API
  slug: dp-bohrium-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dp/refs/heads/main/openapi/dp-bohrium-project-api-openapi.yml
- filename: dp-bohrium-scholar-search-api-openapi.yml
  format: yaml
  label: DP Technology (Bohrium) 学者搜索 (bohrium-scholar-search) API
  slug: dp-bohrium-scholar-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dp/refs/heads/main/openapi/dp-bohrium-scholar-search-api-openapi.yml
- filename: dp-bohrium-sciencepedia-api-openapi.yml
  format: yaml
  label: DP Technology (Bohrium) 科学百科 (bohrium-sciencepedia) API
  slug: dp-bohrium-sciencepedia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dp/refs/heads/main/openapi/dp-bohrium-sciencepedia-api-openapi.yml
- filename: dp-bohrium-tools-api-openapi.yml
  format: yaml
  label: DP Technology (Bohrium) 科学工具库 (bohrium-tools) API
  slug: dp-bohrium-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dp/refs/heads/main/openapi/dp-bohrium-tools-api-openapi.yml
- filename: dp-bohrium-web-search-api-openapi.yml
  format: yaml
  label: DP Technology (Bohrium) 网页搜索 (bohrium-web-search) API
  slug: dp-bohrium-web-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dp/refs/heads/main/openapi/dp-bohrium-web-search-api-openapi.yml
- filename: dp-pdf-bohrium-pdf-parser-api-openapi.yml
  format: yaml
  label: DP Technology (Bohrium) PDF 解析 (bohrium-pdf-parser) API
  slug: dp-pdf-bohrium-pdf-parser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dp/refs/heads/main/openapi/dp-pdf-bohrium-pdf-parser-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dp Authentication
name_suffix: Authentication
oauth_flows: []
overview: DP Technology (Bohrium) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DP Technology (Bohrium)
provider_slug: dp
scheme_count: 1
schemes:
- description: Bohrium AccessKey，环境变量 BOHR_ACCESS_KEY，作为 Bearer token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dp-bohrium-openapi.json
  type: http
slug: dp-authentication
source_filename: dp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/dp-bohrium-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bohrium AccessKey，环境变量 BOHR_ACCESS_KEY，作为 Bearer token\n  sources:\n  - openapi/dp-bohrium-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dp/refs/heads/main/authentication/dp-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI for Science
- Scientific Computing
- Molecular Simulation
- Drug Discovery
- Materials Science
- Research Cloud
- Machine-Learning
- HPC
---
