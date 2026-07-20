---
api_key_in: []
api_specs:
- filename: epignosis-talentlms-efront-talentcards-efront-openapi-original.json
  format: json
  label: eFront API
  slug: efront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epignosis-talentlms-efront-talentcards/refs/heads/main/openapi/epignosis-talentlms-efront-talentcards-efront-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Epignosis Talentlms Efront Talentcards Authentication
name_suffix: Authentication
oauth_flows: []
overview: Epignosis (TalentLMS, eFront, TalentCards) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Epignosis (TalentLMS, eFront, TalentCards)
provider_slug: epignosis-talentlms-efront-talentcards
scheme_count: 1
schemes:
- description: API key supplied as the HTTP Basic auth username with a blank password. Confirmed for eFront (OpenAPI securitySchemes.basicAuth) and documented identically for TalentLMS and TalentCards.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/epignosis-talentlms-efront-talentcards-efront-openapi-original.json
  type: http
slug: epignosis-talentlms-efront-talentcards-authentication
source_filename: epignosis-talentlms-efront-talentcards-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/epignosis-talentlms-efront-talentcards-efront-openapi-original.json\ndocs: https://market.talentlms.com/pages/docs/TalentLMS-API-Documentation.pdf\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  model: >-\n    All three Epignosis products authenticate with a single API key sent over HTTP Basic\n    auth: the API key is the username and the password is left blank. Keys are issued\n    per tenant/installation by a super-administrator and must be sent over HTTPS\n    (TalentLMS rejects plain HTTP from API v4.14+). There is no OAuth, no per-user token,\n    and no scope surface.\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    API key supplied as the HTTP Basic auth username with a blank password. Confirmed\n    for eFront (OpenAPI securitySchemes.basicAuth) and documented identically for\n    TalentLMS and TalentCards.\n  sources:\n  - openapi/epignosis-talentlms-efront-talentcards-efront-openapi-original.json\n\
  products:\n- product: TalentLMS\n  scheme: http-basic-apikey\n  key_location: username\n  password: blank\n  key_management: Account & Settings -> Basic settings (super-admin only)\n  transport: https-required\n  docs: https://market.talentlms.com/pages/docs/TalentLMS-API-Documentation.pdf\n- product: eFront (efrontPRO)\n  scheme: http-basic-apikey\n  key_location: username\n  password: blank\n  key_management: admin -> system settings -> integrations -> API\n  docs: https://app.swaggerhub.com/apis/Epignosis/Efront-API/1.0.0\n- product: TalentCards\n  scheme: http-basic-apikey\n  key_location: username\n  password: blank\n  docs: https://github.com/epignosis/talentcards-api-wrapper\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epignosis-talentlms-efront-talentcards/refs/heads/main/authentication/epignosis-talentlms-efront-talentcards-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Education
- Learning Management System
- LMS
- Training
- eLearning
- Microlearning
- Corporate Training
- SaaS
---
