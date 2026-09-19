---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: upgrad-admin-controller-api-openapi.yml
  format: yaml
  label: upGrad Admin Controller API
  slug: upgrad-admin-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/openapi/upgrad-admin-controller-api-openapi.yml
- filename: upgrad-business-type-controller-api-openapi.yml
  format: yaml
  label: upGrad Business Type Controller API
  slug: upgrad-business-type-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/openapi/upgrad-business-type-controller-api-openapi.yml
- filename: upgrad-commission-rule-controller-api-openapi.yml
  format: yaml
  label: upGrad Commission Rule Controller API
  slug: upgrad-commission-rule-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/openapi/upgrad-commission-rule-controller-api-openapi.yml
- filename: upgrad-form-config-controller-api-openapi.yml
  format: yaml
  label: upGrad Form Config Controller API
  slug: upgrad-form-config-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/openapi/upgrad-form-config-controller-api-openapi.yml
- filename: upgrad-leader-board-controller-api-openapi.yml
  format: yaml
  label: upGrad Leader Board Controller API
  slug: upgrad-leader-board-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/openapi/upgrad-leader-board-controller-api-openapi.yml
- filename: upgrad-learner-invoice-credit-note-controller-api-openapi.yml
  format: yaml
  label: upGrad Learner Invoice Credit Note Controller API
  slug: upgrad-learner-invoice-credit-note-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/openapi/upgrad-learner-invoice-credit-note-controller-api-openapi.yml
- filename: upgrad-login-list-controller-api-openapi.yml
  format: yaml
  label: upGrad Login List Controller API
  slug: upgrad-login-list-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/openapi/upgrad-login-list-controller-api-openapi.yml
- filename: upgrad-login-list-upload-controller-api-openapi.yml
  format: yaml
  label: upGrad Login List Upload Controller API
  slug: upgrad-login-list-upload-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/openapi/upgrad-login-list-upload-controller-api-openapi.yml
- filename: upgrad-master-data-controller-api-openapi.yml
  format: yaml
  label: upGrad Master Data Controller API
  slug: upgrad-master-data-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/openapi/upgrad-master-data-controller-api-openapi.yml
- filename: upgrad-micro-interaction-notification-controller-api-openapi.yml
  format: yaml
  label: upGrad Micro Interaction Notification Controller API
  slug: upgrad-micro-interaction-notification-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/openapi/upgrad-micro-interaction-notification-controller-api-openapi.yml
- filename: upgrad-partner-controller-api-openapi.yml
  format: yaml
  label: upGrad Partner Controller API
  slug: upgrad-partner-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/openapi/upgrad-partner-controller-api-openapi.yml
- filename: upgrad-partner-document-controller-api-openapi.yml
  format: yaml
  label: upGrad Partner Document Controller API
  slug: upgrad-partner-document-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/openapi/upgrad-partner-document-controller-api-openapi.yml
- filename: upgrad-partner-invoice-credit-note-controller-api-openapi.yml
  format: yaml
  label: upGrad Partner Invoice Credit Note Controller API
  slug: upgrad-partner-invoice-credit-note-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/openapi/upgrad-partner-invoice-credit-note-controller-api-openapi.yml
- filename: upgrad-program-key-cache-controller-api-openapi.yml
  format: yaml
  label: upGrad Program Key Cache Controller API
  slug: upgrad-program-key-cache-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/openapi/upgrad-program-key-cache-controller-api-openapi.yml
- filename: upgrad-prospect-controller-api-openapi.yml
  format: yaml
  label: upGrad Prospect Controller API
  slug: upgrad-prospect-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/openapi/upgrad-prospect-controller-api-openapi.yml
- filename: upgrad-status-controller-api-openapi.yml
  format: yaml
  label: upGrad Status Controller API
  slug: upgrad-status-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/openapi/upgrad-status-controller-api-openapi.yml
- filename: upgrad-store-controller-api-openapi.yml
  format: yaml
  label: upGrad Store Controller API
  slug: upgrad-store-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/openapi/upgrad-store-controller-api-openapi.yml
- filename: upgrad-team-member-controller-api-openapi.yml
  format: yaml
  label: upGrad Team Member Controller API
  slug: upgrad-team-member-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/openapi/upgrad-team-member-controller-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Upgrad Authentication
name_suffix: Authentication
oauth_flows: []
overview: upGrad secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: upGrad
provider_slug: upgrad
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: Authorization
  scheme: bearer
  sources:
  - openapi/upgrad-learner-analytics-openapi.yml
  type: http
- in: header
  name: AUTH-TOKEN
  parameter: AUTH-TOKEN
  sources:
  - openapi/upgrad-partner-openapi.yml
  type: apiKey
slug: upgrad-authentication
source_filename: upgrad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: derived\nsource: openapi/upgrad-learner-analytics-openapi.yml, openapi/upgrad-partner-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: Authorization\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/upgrad-learner-analytics-openapi.yml\n- name: AUTH-TOKEN\n  type: apiKey\n  in: header\n  parameter: AUTH-TOKEN\n  sources:\n  - openapi/upgrad-partner-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/authentication/upgrad-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Education
- EdTech
- Online Learning
- Higher Education
- Certification
- Learning Analytics
- Partner Management
- India
---
