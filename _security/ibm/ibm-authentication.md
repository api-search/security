---
api_key_in: []
api_specs:
- filename: assistant-v2.json
  format: json
  label: IBM Watson Assistant
  slug: ibm-watson-assistant
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/watson-developer-cloud/api-spec/master/assistant/assistant-v2.json
- filename: natural-language-understanding.json
  format: json
  label: IBM Watson Natural Language Understanding
  slug: ibm-watson-natural-language-understanding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/watson-developer-cloud/api-spec/master/natural-language-understanding/natural-language-understanding.json
- filename: language-translator.json
  format: json
  label: IBM Watson Language Translator
  slug: ibm-watson-language-translator
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/watson-developer-cloud/api-spec/master/language-translator/language-translator.json
- filename: speech-to-text.json
  format: json
  label: IBM Watson Speech to Text
  slug: ibm-watson-speech-to-text
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/watson-developer-cloud/api-spec/master/speech-to-text/speech-to-text.json
- filename: text-to-speech.json
  format: json
  label: IBM Watson Text to Speech
  slug: ibm-watson-text-to-speech
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/watson-developer-cloud/api-spec/master/text-to-speech/text-to-speech.json
- filename: ibm-cloud-iam.yml
  format: yaml
  label: IBM Cloud IAM Identity Services
  slug: ibm-cloud-iam-identity-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm/refs/heads/main/openapi/ibm-cloud-iam.yml
- filename: ibm-cloud-iam.yml
  format: yaml
  label: IBM IAM Policy Management
  slug: ibm-iam-policy-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm/refs/heads/main/openapi/ibm-cloud-iam.yml
- filename: ibm-cloud-iam.yml
  format: yaml
  label: IBM IAM Access Groups
  slug: ibm-iam-access-groups
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm/refs/heads/main/openapi/ibm-cloud-iam.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ibm Authentication
name_suffix: Authentication
oauth_flows: []
overview: IBM secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IBM
provider_slug: ibm
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'IAM access token obtained from the /identity/token endpoint. Pass as Authorization: Bearer <token>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ibm-cloud-iam.yml
  type: http
slug: ibm-authentication
source_filename: ibm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ibm-cloud-iam.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'IAM access token obtained from the /identity/token endpoint. Pass as Authorization:\n    Bearer <token>.'\n  sources:\n  - openapi/ibm-cloud-iam.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibm/refs/heads/main/authentication/ibm-authentication.yml
summary_line: http · 1 scheme
tags:
- API Management
- Artificial Intelligence
- Billing
- Cloud Computing
- Containers
- Data Governance
- Databases
- DevOps
- Enterprise
- Generative AI
- Hybrid Cloud
- Infrastructure
- Machine Learning
- Networking
- Observability
- Security
- Serverless
- Storage
- Watson
- Watsonx
- Fortune 100
---
