---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ozonetel-agent-api-openapi.yml
  format: yaml
  label: Ozonetel Agent API
  slug: ozonetel-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-agent-api-openapi.yml
- filename: ozonetel-aht-api-openapi.yml
  format: yaml
  label: Ozonetel AHT API
  slug: ozonetel-aht-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-aht-api-openapi.yml
- filename: ozonetel-campaign-api-openapi.yml
  format: yaml
  label: Ozonetel Campaign API
  slug: ozonetel-campaign-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-campaign-api-openapi.yml
- filename: ozonetel-campaign-reports-api-openapi.yml
  format: yaml
  label: Ozonetel Campaign Reports API
  slug: ozonetel-campaign-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-campaign-reports-api-openapi.yml
- filename: ozonetel-chat-campaign-api-openapi.yml
  format: yaml
  label: Ozonetel Chat Campaign API
  slug: ozonetel-chat-campaign-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-chat-campaign-api-openapi.yml
- filename: ozonetel-default-api-openapi.yml
  format: yaml
  label: Ozonetel Default API
  slug: ozonetel-default-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-default-api-openapi.yml
- filename: ozonetel-disposition-api-openapi.yml
  format: yaml
  label: Ozonetel Disposition API
  slug: ozonetel-disposition-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-disposition-api-openapi.yml
- filename: ozonetel-reports-api-openapi.yml
  format: yaml
  label: Ozonetel Reports API
  slug: ozonetel-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-reports-api-openapi.yml
- filename: ozonetel-sms-api-openapi.yml
  format: yaml
  label: Ozonetel SMS API
  slug: ozonetel-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-sms-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Ozonetel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ozonetel secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ozonetel
provider_slug: ozonetel
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ozonetel-add-campaign-data-token-authentication-api-openapi.yml
  - openapi/ozonetel-agent-details-java-token-api-openapi.yml
  - openapi/ozonetel-agent-manual-dial-java-token-api-openapi.yml
  - openapi/ozonetel-agent-manual-dial-skill-token-java-api-openapi.yml
  - openapi/ozonetel-agent-state-summary-token-auth-api-openapi.yml
  - openapi/ozonetel-available-campaigns-token-api-openapi.yml
  - openapi/ozonetel-average-handling-time-token-authentication-api-openapi.yml
  - openapi/ozonetel-call-control-in-conference-java-token-api-openapi.yml
  - openapi/ozonetel-campaign-phone-number-lookup-token-auth-api-openapi.yml
  - openapi/ozonetel-create-agent-java-token-api-openapi.yml
  - openapi/ozonetel-create-block-number-group-java-token-api-openapi.yml
  - openapi/ozonetel-create-chat-campaign-api-token-auth-api-openapi.yml
  - openapi/ozonetel-create-phone-number-java-token-api-openapi.yml
  - openapi/ozonetel-delete-agent-java-token-api-openapi.yml
  - openapi/ozonetel-delete-block-number-grp-java-api-openapi.yml
  - openapi/ozonetel-delete-campaign-data-java-token-api-openapi.yml
  - openapi/ozonetel-delete-chat-campaign-api-token-auth-api-openapi.yml
  - openapi/ozonetel-delete-phone-number-java-token-api-openapi.yml
  - openapi/ozonetel-delete-schedule-campaign-data-java-token-api-openapi.yml
  - openapi/ozonetel-deletebulkdata-api-openapi.yml
  - openapi/ozonetel-edit-agent-details-java-token-api-openapi.yml
  - openapi/ozonetel-edit-phone-number-java-token-api-openapi.yml
  - openapi/ozonetel-fetch-cdr-by-pagination-token-1-api-openapi.yml
  - openapi/ozonetel-fetch-cdr-by-ucid-token-1-api-openapi.yml
  - openapi/ozonetel-fetch-cdr-details-token-1-api-openapi.yml
  - openapi/ozonetel-get-abandon-calls-token-auth-api-openapi.yml
  - openapi/ozonetel-get-block-number-group-java-token-api-openapi.yml
  - openapi/ozonetel-get-campaign-status-token-api-openapi.yml
  - openapi/ozonetel-get-customer-hold-data-cdr-token-api-openapi.yml
  - openapi/ozonetel-get-disposition-list-dispositionv2-token-auth-api-openapi.yml
  - openapi/ozonetel-get-phone-number-details-token-api-openapi.yml
  - openapi/ozonetel-phone-manual-dial-java-token-api-openapi.yml
  - openapi/ozonetel-phone-manual-dial-skillwise-token-api-openapi.yml
  - openapi/ozonetel-release-agent-phone-number-token-auth-api-openapi.yml
  - openapi/ozonetel-schedule-campaign-data-java-token-api-openapi.yml
  - openapi/ozonetel-set-campaign-status-token-1-api-openapi.yml
  - openapi/ozonetel-set-disposition-dispositionv2-token-auth-api-openapi.yml
  - openapi/ozonetel-update-block-number-group-java-token-api-openapi.yml
  - openapi/ozonetel-update-chat-campaign-api-token-auth-api-openapi.yml
  type: http
- name: basicAuth
  scheme: basic
  sources:
  - openapi/ozonetel-agent-authentication-api-openapi.yml
  type: http
slug: ozonetel-authentication
source_filename: ozonetel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: derived\nsource: openapi/ozonetel-add-campaign-data-token-authentication-api-openapi.yml, openapi/ozonetel-agent-authentication-api-openapi.yml,\n  openapi/ozonetel-agent-details-java-token-api-openapi.yml, openapi/ozonetel-agent-manual-dial-java-token-api-openapi.yml,\n  openapi/ozonetel-agent-manual-dial-skill-token-java-api-openapi.yml, openapi/ozonetel-agent-state-summary-token-auth-api-openapi.yml,\n  openapi/ozonetel-available-campaigns-token-api-openapi.yml, openapi/ozonetel-average-handling-time-token-authentication-api-openapi.yml,\n  openapi/ozonetel-call-control-in-conference-java-token-api-openapi.yml, openapi/ozonetel-campaign-phone-number-lookup-token-auth-api-openapi.yml,\n  openapi/ozonetel-create-agent-java-token-api-openapi.yml, openapi/ozonetel-create-block-number-group-java-token-api-openapi.yml\n  ...\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/ozonetel-add-campaign-data-token-authentication-api-openapi.yml\n\
  \  - openapi/ozonetel-agent-details-java-token-api-openapi.yml\n  - openapi/ozonetel-agent-manual-dial-java-token-api-openapi.yml\n  - openapi/ozonetel-agent-manual-dial-skill-token-java-api-openapi.yml\n  - openapi/ozonetel-agent-state-summary-token-auth-api-openapi.yml\n  - openapi/ozonetel-available-campaigns-token-api-openapi.yml\n  - openapi/ozonetel-average-handling-time-token-authentication-api-openapi.yml\n  - openapi/ozonetel-call-control-in-conference-java-token-api-openapi.yml\n  - openapi/ozonetel-campaign-phone-number-lookup-token-auth-api-openapi.yml\n  - openapi/ozonetel-create-agent-java-token-api-openapi.yml\n  - openapi/ozonetel-create-block-number-group-java-token-api-openapi.yml\n  - openapi/ozonetel-create-chat-campaign-api-token-auth-api-openapi.yml\n  - openapi/ozonetel-create-phone-number-java-token-api-openapi.yml\n  - openapi/ozonetel-delete-agent-java-token-api-openapi.yml\n  - openapi/ozonetel-delete-block-number-grp-java-api-openapi.yml\n  - openapi/ozonetel-delete-campaign-data-java-token-api-openapi.yml\n\
  \  - openapi/ozonetel-delete-chat-campaign-api-token-auth-api-openapi.yml\n  - openapi/ozonetel-delete-phone-number-java-token-api-openapi.yml\n  - openapi/ozonetel-delete-schedule-campaign-data-java-token-api-openapi.yml\n  - openapi/ozonetel-deletebulkdata-api-openapi.yml\n  - openapi/ozonetel-edit-agent-details-java-token-api-openapi.yml\n  - openapi/ozonetel-edit-phone-number-java-token-api-openapi.yml\n  - openapi/ozonetel-fetch-cdr-by-pagination-token-1-api-openapi.yml\n  - openapi/ozonetel-fetch-cdr-by-ucid-token-1-api-openapi.yml\n  - openapi/ozonetel-fetch-cdr-details-token-1-api-openapi.yml\n  - openapi/ozonetel-get-abandon-calls-token-auth-api-openapi.yml\n  - openapi/ozonetel-get-block-number-group-java-token-api-openapi.yml\n  - openapi/ozonetel-get-campaign-status-token-api-openapi.yml\n  - openapi/ozonetel-get-customer-hold-data-cdr-token-api-openapi.yml\n  - openapi/ozonetel-get-disposition-list-dispositionv2-token-auth-api-openapi.yml\n  - openapi/ozonetel-get-phone-number-details-token-api-openapi.yml\n\
  \  - openapi/ozonetel-phone-manual-dial-java-token-api-openapi.yml\n  - openapi/ozonetel-phone-manual-dial-skillwise-token-api-openapi.yml\n  - openapi/ozonetel-release-agent-phone-number-token-auth-api-openapi.yml\n  - openapi/ozonetel-schedule-campaign-data-java-token-api-openapi.yml\n  - openapi/ozonetel-set-campaign-status-token-1-api-openapi.yml\n  - openapi/ozonetel-set-disposition-dispositionv2-token-auth-api-openapi.yml\n  - openapi/ozonetel-update-block-number-group-java-token-api-openapi.yml\n  - openapi/ozonetel-update-chat-campaign-api-token-auth-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/ozonetel-agent-authentication-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/ozonetel/authentication/ozonetel-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- CX Platform
- Cloud Communications
- Contact Center
- API
---
