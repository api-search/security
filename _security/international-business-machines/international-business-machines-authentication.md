---
api_key_in: []
api_specs:
- filename: ibm-watsonx-ai-openapi.yml
  format: yaml
  label: IBM Watsonx.ai API
  slug: watsonx-ai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-watsonx-ai-openapi.yml
- filename: ibm-watsonx-assistant-openapi.yml
  format: yaml
  label: IBM Watsonx Assistant V2 API
  slug: watsonx-assistant
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-watsonx-assistant-openapi.yml
- filename: ibm-natural-language-understanding-openapi.yml
  format: yaml
  label: IBM Natural Language Understanding API
  slug: natural-language-understanding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-natural-language-understanding-openapi.yml
- filename: ibm-speech-to-text-openapi.yml
  format: yaml
  label: IBM Speech to Text API
  slug: speech-to-text
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-speech-to-text-openapi.yml
- filename: ibm-text-to-speech-openapi.yml
  format: yaml
  label: IBM Text to Speech API
  slug: text-to-speech
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-text-to-speech-openapi.yml
- filename: ibm-cloud-object-storage-openapi.yml
  format: yaml
  label: IBM Cloud Object Storage API
  slug: cloud-object-storage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-cloud-object-storage-openapi.yml
- filename: ibm-kubernetes-service-openapi.yml
  format: yaml
  label: IBM Cloud Kubernetes Service API
  slug: kubernetes-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-kubernetes-service-openapi.yml
- filename: ibm-vpc-openapi.yml
  format: yaml
  label: IBM Cloud VPC API
  slug: vpc
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-vpc-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: International Business Machines Authentication
name_suffix: Authentication
oauth_flows: []
overview: International Business Machines secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: International Business Machines
provider_slug: international-business-machines
scheme_count: 1
schemes:
- bearerFormat: IAM Token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ibm-cloud-object-storage-openapi.yml
  - openapi/ibm-kubernetes-service-openapi.yml
  - openapi/ibm-natural-language-understanding-openapi.yml
  - openapi/ibm-speech-to-text-openapi.yml
  - openapi/ibm-text-to-speech-openapi.yml
  - openapi/ibm-vpc-openapi.yml
  - openapi/ibm-watsonx-ai-openapi.yml
  - openapi/ibm-watsonx-assistant-openapi.yml
  type: http
slug: international-business-machines-authentication
source_filename: international-business-machines-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ibm-cloud-object-storage-openapi.yml, openapi/ibm-kubernetes-service-openapi.yml,\n  openapi/ibm-natural-language-understanding-openapi.yml, openapi/ibm-speech-to-text-openapi.yml,\n  openapi/ibm-text-to-speech-openapi.yml, openapi/ibm-vpc-openapi.yml, openapi/ibm-watsonx-ai-openapi.yml,\n  openapi/ibm-watsonx-assistant-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: IAM Token\n  sources:\n  - openapi/ibm-cloud-object-storage-openapi.yml\n  - openapi/ibm-kubernetes-service-openapi.yml\n  - openapi/ibm-natural-language-understanding-openapi.yml\n  - openapi/ibm-speech-to-text-openapi.yml\n  - openapi/ibm-text-to-speech-openapi.yml\n  - openapi/ibm-vpc-openapi.yml\n  - openapi/ibm-watsonx-ai-openapi.yml\n  - openapi/ibm-watsonx-assistant-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/authentication/international-business-machines-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Cloud
- Enterprise
- IBM
---
