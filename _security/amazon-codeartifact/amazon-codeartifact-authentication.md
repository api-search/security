---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-codeartifact-domain-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Domain API
  slug: amazon-codeartifact-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-domain-api-openapi.yml
- filename: amazon-codeartifact-domains-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Domains API
  slug: amazon-codeartifact-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-domains-api-openapi.yml
- filename: amazon-codeartifact-package-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Package API
  slug: amazon-codeartifact-package-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-package-api-openapi.yml
- filename: amazon-codeartifact-repositories-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Repositories API
  slug: amazon-codeartifact-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-repositories-api-openapi.yml
- filename: amazon-codeartifact-repository-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Repository API
  slug: amazon-codeartifact-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-repository-api-openapi.yml
- filename: amazon-codeartifact-authorization-token-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Authorization Token API
  slug: amazon-codeartifact-authorization-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-authorization-token-api-openapi.yml
- filename: amazon-codeartifact-packages-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Packages API
  slug: amazon-codeartifact-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-packages-api-openapi.yml
- filename: amazon-codeartifact-tag-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Tag API
  slug: amazon-codeartifact-tag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-tag-api-openapi.yml
- filename: amazon-codeartifact-tags-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Tags API
  slug: amazon-codeartifact-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-tags-api-openapi.yml
- filename: amazon-codeartifact-untag-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Untag API
  slug: amazon-codeartifact-untag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-untag-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Codeartifact Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon CodeArtifact secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-codeartifact-openapi-original.yaml
  type: apiKey
slug: amazon-codeartifact-authentication
source_filename: amazon-codeartifact-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-codeartifact-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-codeartifact-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/authentication/amazon-codeartifact-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon
- Artifact Repository
- Package Management
- DevOps
- Software Supply Chain
- npm
- Maven
- PyPI
- NuGet
- Developer Tools
---
