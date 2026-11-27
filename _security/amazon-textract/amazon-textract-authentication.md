---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-textract-async-operations-api-openapi.yml
  format: yaml
  label: Amazon Textract Async Operations API
  slug: amazon-textract-async-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-textract/openapi/amazon-textract-async-operations-api-openapi.yml
- filename: amazon-textract-document-analysis-api-openapi.yml
  format: yaml
  label: Amazon Textract Document Analysis API
  slug: amazon-textract-document-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-textract/openapi/amazon-textract-document-analysis-api-openapi.yml
- filename: amazon-textract-expense-analysis-api-openapi.yml
  format: yaml
  label: Amazon Textract Expense Analysis API
  slug: amazon-textract-expense-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-textract/openapi/amazon-textract-expense-analysis-api-openapi.yml
- filename: amazon-textract-id-analysis-api-openapi.yml
  format: yaml
  label: Amazon Textract ID Analysis API
  slug: amazon-textract-id-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-textract/openapi/amazon-textract-id-analysis-api-openapi.yml
- filename: amazon-textract-text-detection-api-openapi.yml
  format: yaml
  label: Amazon Textract Text Detection API
  slug: amazon-textract-text-detection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-textract/openapi/amazon-textract-text-detection-api-openapi.yml
- filename: amazon-textract-adapter-api-openapi.yml
  format: yaml
  label: Amazon Textract Textract Adapter API
  slug: amazon-textract-adapter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-textract/openapi/amazon-textract-adapter-api-openapi.yml
- filename: amazon-textract-adapter-version-api-openapi.yml
  format: yaml
  label: Amazon Textract Textract Adapter Version API
  slug: amazon-textract-adapter-version-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-textract/openapi/amazon-textract-adapter-version-api-openapi.yml
- filename: amazon-textract-operations-api-openapi.yml
  format: yaml
  label: Amazon Textract Textract Operations API
  slug: amazon-textract-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-textract/openapi/amazon-textract-operations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Textract Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Textract secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Textract
provider_slug: amazon-textract
scheme_count: 1
schemes:
- description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256 signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary credentials). Not a bearer token.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-textract-adapter-api-openapi.yml
  - openapi/amazon-textract-adapter-version-api-openapi.yml
  - openapi/amazon-textract-async-operations-api-openapi.yml
  - openapi/amazon-textract-document-analysis-api-openapi.yml
  - openapi/amazon-textract-expense-analysis-api-openapi.yml
  - openapi/amazon-textract-id-analysis-api-openapi.yml
  - openapi/amazon-textract-operations-api-openapi.yml
  - openapi/amazon-textract-text-detection-api-openapi.yml
  type: apiKey
slug: amazon-textract-authentication
source_filename: amazon-textract-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/amazon-textract-adapter-api-openapi.yml, openapi/amazon-textract-adapter-version-api-openapi.yml,\n  openapi/amazon-textract-async-operations-api-openapi.yml, openapi/amazon-textract-document-analysis-api-openapi.yml,\n  openapi/amazon-textract-expense-analysis-api-openapi.yml, openapi/amazon-textract-id-analysis-api-openapi.yml,\n  openapi/amazon-textract-operations-api-openapi.yml, openapi/amazon-textract-text-detection-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256\n    signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary\n    credentials). Not a bearer token.\n  sources:\n  - openapi/amazon-textract-adapter-api-openapi.yml\n  - openapi/amazon-textract-adapter-version-api-openapi.yml\n\
  \  - openapi/amazon-textract-async-operations-api-openapi.yml\n  - openapi/amazon-textract-document-analysis-api-openapi.yml\n  - openapi/amazon-textract-expense-analysis-api-openapi.yml\n  - openapi/amazon-textract-id-analysis-api-openapi.yml\n  - openapi/amazon-textract-operations-api-openapi.yml\n  - openapi/amazon-textract-text-detection-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-textract/authentication/amazon-textract-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Document Processing
- Machine Learning
- OCR
---
