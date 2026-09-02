---
api_key_in:
- header
api_specs:
- filename: v1
  format: yaml
  label: Act! Web API
  slug: web-api
  spec_type: OpenAPI
  url: https://apimta.act.com/act.web.api/swagger/docs/v1
- filename: act-activityseries-api-openapi.yml
  format: yaml
  label: Act! CRM Activity Series API
  slug: act-activityseries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/openapi/act-activityseries-api-openapi.yml
- filename: act-customentities-api-openapi.yml
  format: yaml
  label: Act! CRM Custom Entities API
  slug: act-customentities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/openapi/act-customentities-api-openapi.yml
- filename: act-documenttypes-api-openapi.yml
  format: yaml
  label: Act! CRM Document Types API
  slug: act-documenttypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/openapi/act-documenttypes-api-openapi.yml
- filename: act-historytypes-api-openapi.yml
  format: yaml
  label: Act! CRM History Types API
  slug: act-historytypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/openapi/act-historytypes-api-openapi.yml
- filename: act-marketingautomations-api-openapi.yml
  format: yaml
  label: Act! CRM Marketing Automations API
  slug: act-marketingautomations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/openapi/act-marketingautomations-api-openapi.yml
- filename: act-metadatainfo-api-openapi.yml
  format: yaml
  label: Act! CRM Metadata Info API
  slug: act-metadatainfo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/openapi/act-metadatainfo-api-openapi.yml
- filename: act-secondarycontacts-api-openapi.yml
  format: yaml
  label: Act! CRM Secondary Contacts API
  slug: act-secondarycontacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/openapi/act-secondarycontacts-api-openapi.yml
- filename: act-supplementalfiles-api-openapi.yml
  format: yaml
  label: Act! CRM Supplemental Files API
  slug: act-supplementalfiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/openapi/act-supplementalfiles-api-openapi.yml
- filename: act-syncdata-api-openapi.yml
  format: yaml
  label: Act! CRM Sync Data API
  slug: act-syncdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/openapi/act-syncdata-api-openapi.yml
- filename: act-tasktypes-api-openapi.yml
  format: yaml
  label: Act! CRM Task Types API
  slug: act-tasktypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/openapi/act-tasktypes-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Act Authentication
name_suffix: Authentication
oauth_flows: []
overview: Act! CRM secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Act! CRM
provider_slug: act
scheme_count: 3
schemes:
- description: HTTP Basic credentials (Act! user name and password, RFC 7617) presented to GET /authorize together with the Act-Database-Name header to mint a JWT bearer token.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/act-activity-series-api-openapi.yml
  - openapi/act-analytics-api-openapi.yml
  - openapi/act-calendar-api-openapi.yml
  - openapi/act-companies-api-openapi.yml
  - openapi/act-configurations-api-openapi.yml
  - openapi/act-contacts-api-openapi.yml
  - openapi/act-cors-api-openapi.yml
  - openapi/act-custom-entities-api-openapi.yml
  - openapi/act-database-api-openapi.yml
  - openapi/act-document-types-api-openapi.yml
  - openapi/act-documents-api-openapi.yml
  - openapi/act-geographics-api-openapi.yml
  - openapi/act-groups-api-openapi.yml
  - openapi/act-history-api-openapi.yml
  - openapi/act-history-types-api-openapi.yml
  - openapi/act-import-api-openapi.yml
  - openapi/act-marketing-automations-api-openapi.yml
  - openapi/act-metadata-info-api-openapi.yml
  - openapi/act-notes-api-openapi.yml
  - openapi/act-opportunities-api-openapi.yml
  - openapi/act-preferences-api-openapi.yml
  - openapi/act-products-api-openapi.yml
  - openapi/act-secondary-contacts-api-openapi.yml
  - openapi/act-supplemental-files-api-openapi.yml
  - openapi/act-sync-data-api-openapi.yml
  - openapi/act-system-api-openapi.yml
  - openapi/act-task-types-api-openapi.yml
  - openapi/act-tasks-api-openapi.yml
  - openapi/act-teams-api-openapi.yml
  - openapi/act-users-api-openapi.yml
  - openapi/act-webhooks-api-openapi.yml
  type: http
- bearerFormat: JWT
  description: 'JWT bearer token returned by GET /authorize (RFC 6750). Sent as Authorization: Bearer <token> on every API request.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/act-activity-series-api-openapi.yml
  - openapi/act-analytics-api-openapi.yml
  - openapi/act-calendar-api-openapi.yml
  - openapi/act-companies-api-openapi.yml
  - openapi/act-configurations-api-openapi.yml
  - openapi/act-contacts-api-openapi.yml
  - openapi/act-cors-api-openapi.yml
  - openapi/act-custom-entities-api-openapi.yml
  - openapi/act-database-api-openapi.yml
  - openapi/act-document-types-api-openapi.yml
  - openapi/act-documents-api-openapi.yml
  - openapi/act-geographics-api-openapi.yml
  - openapi/act-groups-api-openapi.yml
  - openapi/act-history-api-openapi.yml
  - openapi/act-history-types-api-openapi.yml
  - openapi/act-import-api-openapi.yml
  - openapi/act-marketing-automations-api-openapi.yml
  - openapi/act-metadata-info-api-openapi.yml
  - openapi/act-notes-api-openapi.yml
  - openapi/act-opportunities-api-openapi.yml
  - openapi/act-preferences-api-openapi.yml
  - openapi/act-products-api-openapi.yml
  - openapi/act-secondary-contacts-api-openapi.yml
  - openapi/act-supplemental-files-api-openapi.yml
  - openapi/act-sync-data-api-openapi.yml
  - openapi/act-system-api-openapi.yml
  - openapi/act-task-types-api-openapi.yml
  - openapi/act-tasks-api-openapi.yml
  - openapi/act-teams-api-openapi.yml
  - openapi/act-users-api-openapi.yml
  - openapi/act-webhooks-api-openapi.yml
  type: http
- description: Name of the Act! database the request is scoped to.
  in: header
  name: actDatabaseName
  parameter: Act-Database-Name
  sources:
  - openapi/act-activity-series-api-openapi.yml
  - openapi/act-analytics-api-openapi.yml
  - openapi/act-calendar-api-openapi.yml
  - openapi/act-companies-api-openapi.yml
  - openapi/act-configurations-api-openapi.yml
  - openapi/act-contacts-api-openapi.yml
  - openapi/act-cors-api-openapi.yml
  - openapi/act-custom-entities-api-openapi.yml
  - openapi/act-database-api-openapi.yml
  - openapi/act-document-types-api-openapi.yml
  - openapi/act-documents-api-openapi.yml
  - openapi/act-geographics-api-openapi.yml
  - openapi/act-groups-api-openapi.yml
  - openapi/act-history-api-openapi.yml
  - openapi/act-history-types-api-openapi.yml
  - openapi/act-import-api-openapi.yml
  - openapi/act-marketing-automations-api-openapi.yml
  - openapi/act-metadata-info-api-openapi.yml
  - openapi/act-notes-api-openapi.yml
  - openapi/act-opportunities-api-openapi.yml
  - openapi/act-preferences-api-openapi.yml
  - openapi/act-products-api-openapi.yml
  - openapi/act-secondary-contacts-api-openapi.yml
  - openapi/act-supplemental-files-api-openapi.yml
  - openapi/act-sync-data-api-openapi.yml
  - openapi/act-system-api-openapi.yml
  - openapi/act-task-types-api-openapi.yml
  - openapi/act-tasks-api-openapi.yml
  - openapi/act-teams-api-openapi.yml
  - openapi/act-users-api-openapi.yml
  - openapi/act-webhooks-api-openapi.yml
  type: apiKey
slug: act-authentication
source_filename: act-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/act-activity-series-api-openapi.yml, openapi/act-analytics-api-openapi.yml,\n  openapi/act-calendar-api-openapi.yml, openapi/act-companies-api-openapi.yml, openapi/act-configurations-api-openapi.yml,\n  openapi/act-contacts-api-openapi.yml, openapi/act-cors-api-openapi.yml, openapi/act-custom-entities-api-openapi.yml,\n  openapi/act-database-api-openapi.yml, openapi/act-document-types-api-openapi.yml, openapi/act-documents-api-openapi.yml,\n  openapi/act-geographics-api-openapi.yml ...\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic credentials (Act! user name and password, RFC 7617) presented to GET\n    /authorize together with the Act-Database-Name header to mint a JWT bearer token.\n  sources:\n  - openapi/act-activity-series-api-openapi.yml\n  - openapi/act-analytics-api-openapi.yml\n  - openapi/act-calendar-api-openapi.yml\n\
  \  - openapi/act-companies-api-openapi.yml\n  - openapi/act-configurations-api-openapi.yml\n  - openapi/act-contacts-api-openapi.yml\n  - openapi/act-cors-api-openapi.yml\n  - openapi/act-custom-entities-api-openapi.yml\n  - openapi/act-database-api-openapi.yml\n  - openapi/act-document-types-api-openapi.yml\n  - openapi/act-documents-api-openapi.yml\n  - openapi/act-geographics-api-openapi.yml\n  - openapi/act-groups-api-openapi.yml\n  - openapi/act-history-api-openapi.yml\n  - openapi/act-history-types-api-openapi.yml\n  - openapi/act-import-api-openapi.yml\n  - openapi/act-marketing-automations-api-openapi.yml\n  - openapi/act-metadata-info-api-openapi.yml\n  - openapi/act-notes-api-openapi.yml\n  - openapi/act-opportunities-api-openapi.yml\n  - openapi/act-preferences-api-openapi.yml\n  - openapi/act-products-api-openapi.yml\n  - openapi/act-secondary-contacts-api-openapi.yml\n  - openapi/act-supplemental-files-api-openapi.yml\n  - openapi/act-sync-data-api-openapi.yml\n  - openapi/act-system-api-openapi.yml\n\
  \  - openapi/act-task-types-api-openapi.yml\n  - openapi/act-tasks-api-openapi.yml\n  - openapi/act-teams-api-openapi.yml\n  - openapi/act-users-api-openapi.yml\n  - openapi/act-webhooks-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'JWT bearer token returned by GET /authorize (RFC 6750). Sent as Authorization:\n    Bearer <token> on every API request.'\n  sources:\n  - openapi/act-activity-series-api-openapi.yml\n  - openapi/act-analytics-api-openapi.yml\n  - openapi/act-calendar-api-openapi.yml\n  - openapi/act-companies-api-openapi.yml\n  - openapi/act-configurations-api-openapi.yml\n  - openapi/act-contacts-api-openapi.yml\n  - openapi/act-cors-api-openapi.yml\n  - openapi/act-custom-entities-api-openapi.yml\n  - openapi/act-database-api-openapi.yml\n  - openapi/act-document-types-api-openapi.yml\n  - openapi/act-documents-api-openapi.yml\n  - openapi/act-geographics-api-openapi.yml\n  - openapi/act-groups-api-openapi.yml\n\
  \  - openapi/act-history-api-openapi.yml\n  - openapi/act-history-types-api-openapi.yml\n  - openapi/act-import-api-openapi.yml\n  - openapi/act-marketing-automations-api-openapi.yml\n  - openapi/act-metadata-info-api-openapi.yml\n  - openapi/act-notes-api-openapi.yml\n  - openapi/act-opportunities-api-openapi.yml\n  - openapi/act-preferences-api-openapi.yml\n  - openapi/act-products-api-openapi.yml\n  - openapi/act-secondary-contacts-api-openapi.yml\n  - openapi/act-supplemental-files-api-openapi.yml\n  - openapi/act-sync-data-api-openapi.yml\n  - openapi/act-system-api-openapi.yml\n  - openapi/act-task-types-api-openapi.yml\n  - openapi/act-tasks-api-openapi.yml\n  - openapi/act-teams-api-openapi.yml\n  - openapi/act-users-api-openapi.yml\n  - openapi/act-webhooks-api-openapi.yml\n- name: actDatabaseName\n  type: apiKey\n  in: header\n  parameter: Act-Database-Name\n  description: Name of the Act! database the request is scoped to.\n  sources:\n  - openapi/act-activity-series-api-openapi.yml\n\
  \  - openapi/act-analytics-api-openapi.yml\n  - openapi/act-calendar-api-openapi.yml\n  - openapi/act-companies-api-openapi.yml\n  - openapi/act-configurations-api-openapi.yml\n  - openapi/act-contacts-api-openapi.yml\n  - openapi/act-cors-api-openapi.yml\n  - openapi/act-custom-entities-api-openapi.yml\n  - openapi/act-database-api-openapi.yml\n  - openapi/act-document-types-api-openapi.yml\n  - openapi/act-documents-api-openapi.yml\n  - openapi/act-geographics-api-openapi.yml\n  - openapi/act-groups-api-openapi.yml\n  - openapi/act-history-api-openapi.yml\n  - openapi/act-history-types-api-openapi.yml\n  - openapi/act-import-api-openapi.yml\n  - openapi/act-marketing-automations-api-openapi.yml\n  - openapi/act-metadata-info-api-openapi.yml\n  - openapi/act-notes-api-openapi.yml\n  - openapi/act-opportunities-api-openapi.yml\n  - openapi/act-preferences-api-openapi.yml\n  - openapi/act-products-api-openapi.yml\n  - openapi/act-secondary-contacts-api-openapi.yml\n  - openapi/act-supplemental-files-api-openapi.yml\n\
  \  - openapi/act-sync-data-api-openapi.yml\n  - openapi/act-system-api-openapi.yml\n  - openapi/act-task-types-api-openapi.yml\n  - openapi/act-tasks-api-openapi.yml\n  - openapi/act-teams-api-openapi.yml\n  - openapi/act-users-api-openapi.yml\n  - openapi/act-webhooks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/authentication/act-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- CRM
- Marketing Automation
- Contact Management
- Sales
- Opportunity Management
- OData
- Small Business
---
