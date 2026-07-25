---
api_key_in:
- header
api_specs:
- filename: amazon-codeartifact-authorization-token-domain-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Authorization Token#domain API
  slug: amazon-codeartifact-authorization-token-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-authorization-token-domain-api-openapi.yml
- filename: amazon-codeartifact-domain-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Domain API
  slug: amazon-codeartifact-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-domain-api-openapi.yml
- filename: amazon-codeartifact-domain-domain-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Domain#domain API
  slug: amazon-codeartifact-domain-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-domain-domain-api-openapi.yml
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
- filename: amazon-codeartifact-package-domain-repository-format-package-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Package#domain&repository&format&package API
  slug: amazon-codeartifact-package-domain-repository-format-package-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-package-domain-repository-format-package-api-openapi.yml
- filename: amazon-codeartifact-packages-domain-repository-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Packages#domain&repository API
  slug: amazon-codeartifact-packages-domain-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-packages-domain-repository-api-openapi.yml
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
- filename: amazon-codeartifact-repository-domain-repository-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Repository#domain&repository API
  slug: amazon-codeartifact-repository-domain-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-repository-domain-repository-api-openapi.yml
- filename: amazon-codeartifact-tag-resourcearn-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Tag#resourceArn API
  slug: amazon-codeartifact-tag-resourcearn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-tag-resourcearn-api-openapi.yml
- filename: amazon-codeartifact-tags-resourcearn-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Tags#resourceArn API
  slug: amazon-codeartifact-tags-resourcearn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-tags-resourcearn-api-openapi.yml
- filename: amazon-codeartifact-untag-resourcearn-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Untag#resourceArn API
  slug: amazon-codeartifact-untag-resourcearn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-untag-resourcearn-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
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
---
