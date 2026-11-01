---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: hmm21-arrival-notice-api-openapi.yml
  format: yaml
  label: HMM Arrival Notice API
  slug: hmm21-arrival-notice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hmm21/openapi/hmm21-arrival-notice-api-openapi.yml
- filename: hmm21-bookings-api-openapi.yml
  format: yaml
  label: HMM Bookings API
  slug: hmm21-bookings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hmm21/openapi/hmm21-bookings-api-openapi.yml
- filename: hmm21-eblcompany-id-requests-api-openapi.yml
  format: yaml
  label: HMM Eblcompany Id Requests API
  slug: hmm21-eblcompany-id-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hmm21/openapi/hmm21-eblcompany-id-requests-api-openapi.yml
- filename: hmm21-kr-nexawave-cert-file-api-openapi.yml
  format: yaml
  label: HMM KR NEXAWAVE CERT FILE API
  slug: hmm21-kr-nexawave-cert-file-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hmm21/openapi/hmm21-kr-nexawave-cert-file-api-openapi.yml
- filename: hmm21-kr-nexawave-class-survey-api-openapi.yml
  format: yaml
  label: HMM KR NEXAWAVE CLASS SURVEY API
  slug: hmm21-kr-nexawave-class-survey-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hmm21/openapi/hmm21-kr-nexawave-class-survey-api-openapi.yml
- filename: hmm21-kr-nexawave-cms-pms-api-openapi.yml
  format: yaml
  label: HMM KR NEXAWAVE CMS PMS API
  slug: hmm21-kr-nexawave-cms-pms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hmm21/openapi/hmm21-kr-nexawave-cms-pms-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hmm21 Authentication
name_suffix: Authentication
oauth_flows: []
overview: HMM secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HMM
provider_slug: hmm21
scheme_count: 1
schemes:
- documentation: 'API keys are issued after sign-up and approval process through the HMM Open API Developer Portal.

    Access tokens can be requested through the "Get Access Token" button on API detail pages.

    '
  in: header
  name: apiKey
  parameter: x-Gateway-APIKey
  sources:
  - openapi/hmm21-arrival-notice-openapi.yml
  - openapi/hmm21-booking-openapi.yml
  - openapi/hmm21-certificate-file-openapi.yml
  - openapi/hmm21-class-survey-status-openapi.yml
  - openapi/hmm21-cms-pms-status-openapi.yml
  - openapi/hmm21-ebl-company-id-openapi.yml
  type: apiKey
slug: hmm21-authentication
source_filename: hmm21-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: searched\nsource: https://apiportal.hmm21.com/info\ndocs: https://apiportal.hmm21.com/info\nnotes: >\n  API uses API key authentication via x-Gateway-APIKey header. Access tokens can be\n  requested through the API portal interface after sign-up and approval process.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-Gateway-APIKey\n  sources:\n  - openapi/hmm21-arrival-notice-openapi.yml\n  - openapi/hmm21-booking-openapi.yml\n  - openapi/hmm21-certificate-file-openapi.yml\n  - openapi/hmm21-class-survey-status-openapi.yml\n  - openapi/hmm21-cms-pms-status-openapi.yml\n  - openapi/hmm21-ebl-company-id-openapi.yml\n  documentation: |\n    API keys are issued after sign-up and approval process through the HMM Open API Developer Portal.\n    Access tokens can be requested through the \"Get Access Token\" button on API detail pages.\n"
source_yaml_url: https://artifacts.apis.io/hmm21/authentication/hmm21-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Shipping
- Logistics
- Container Shipping
- Maritime
- DCSA
- Supply Chain
---
