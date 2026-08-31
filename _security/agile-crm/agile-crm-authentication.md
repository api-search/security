---
api_key_in: []
api_specs:
- filename: agile-crm-campaigns-api-openapi.yml
  format: yaml
  label: Agile CRM Campaigns API
  slug: agile-crm-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/openapi/agile-crm-campaigns-api-openapi.yml
- filename: agile-crm-companies-api-openapi.yml
  format: yaml
  label: Agile CRM Companies API
  slug: agile-crm-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/openapi/agile-crm-companies-api-openapi.yml
- filename: agile-crm-contacts-api-openapi.yml
  format: yaml
  label: Agile CRM Contacts API
  slug: agile-crm-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/openapi/agile-crm-contacts-api-openapi.yml
- filename: agile-crm-deals-api-openapi.yml
  format: yaml
  label: Agile CRM Deals API
  slug: agile-crm-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/openapi/agile-crm-deals-api-openapi.yml
- filename: agile-crm-documents-api-openapi.yml
  format: yaml
  label: Agile CRM Documents API
  slug: agile-crm-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/openapi/agile-crm-documents-api-openapi.yml
- filename: agile-crm-events-api-openapi.yml
  format: yaml
  label: Agile CRM Events API
  slug: agile-crm-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/openapi/agile-crm-events-api-openapi.yml
- filename: agile-crm-helpdesk-api-openapi.yml
  format: yaml
  label: Agile CRM HelpDesk API
  slug: agile-crm-helpdesk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/openapi/agile-crm-helpdesk-api-openapi.yml
- filename: agile-crm-notes-api-openapi.yml
  format: yaml
  label: Agile CRM Notes API
  slug: agile-crm-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/openapi/agile-crm-notes-api-openapi.yml
- filename: agile-crm-tasks-api-openapi.yml
  format: yaml
  label: Agile CRM Tasks API
  slug: agile-crm-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/openapi/agile-crm-tasks-api-openapi.yml
- filename: agile-crm-tracks-api-openapi.yml
  format: yaml
  label: Agile CRM Tracks API
  slug: agile-crm-tracks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/openapi/agile-crm-tracks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Agile Crm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agile CRM secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Agile CRM
provider_slug: agile-crm
scheme_count: 1
schemes:
- case_sensitivity: Agile CRM documents that all data is case-sensitive, including the email used as the Basic username.
  credential_location: Admin Settings > API & Analytics > API Key
  credential_note: 'That screen lists more than one key. The vendor is explicit that only the first one applies: "Use the first one (API Key for REST client) for all the REST API calls." Using another key from the same screen yields HTTP 401.'
  description: 'HTTP Basic authentication. The username is the account holder''s EMAIL ADDRESS and the password is the REST client API key. The vendor states: "This is an HTTPS-only API. Authentications are performed based on the email address of the user and the respective API Key."'
  header: 'Authorization: Basic base64(email:apikey)'
  name: BasicAuth
  scheme: basic
  sources:
  - https://github.com/agilecrm/rest-api/blob/master/README.md
  - openapi/agile-crm-contacts-api-openapi.yml
  tenant_scoping: The credential is bound to a tenant subdomain. Requests must go to https://{domain}.agilecrm.com/dev where {domain} is the account's own subdomain; a key will not authenticate against another tenant's host.
  type: http
slug: agile-crm-authentication
source_filename: agile-crm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://github.com/agilecrm/rest-api/blob/master/README.md#things-to-know\ndocs: https://github.com/agilecrm/rest-api#authentication-\nsummary:\n  types:\n  - http\n  oauth2: false\n  scopes: false\n  rotation_documented: false\n  expiry: none\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication. The username is the account holder's EMAIL ADDRESS and the password is\n    the REST client API key. The vendor states: \"This is an HTTPS-only API. Authentications are\n    performed based on the email address of the user and the respective API Key.\"\n  header: 'Authorization: Basic base64(email:apikey)'\n  credential_location: Admin Settings > API & Analytics > API Key\n  credential_note: >-\n    That screen lists more than one key. The vendor is explicit that only the first one applies:\n    \"Use the first one (API Key for REST client) for all the REST API calls.\" Using\
  \ another key from\n    the same screen yields HTTP 401.\n  tenant_scoping: >-\n    The credential is bound to a tenant subdomain. Requests must go to\n    https://{domain}.agilecrm.com/dev where {domain} is the account's own subdomain; a key will not\n    authenticate against another tenant's host.\n  case_sensitivity: >-\n    Agile CRM documents that all data is case-sensitive, including the email used as the Basic\n    username.\n  sources:\n  - https://github.com/agilecrm/rest-api/blob/master/README.md\n  - openapi/agile-crm-contacts-api-openapi.yml\nposture:\n  privilege_model: full-account\n  per_integration_credentials: false\n  scoped_tokens: false\n  token_expiry: false\n  refresh: false\n  mfa_on_api: false\n  ip_allowlist: false\n  key_rotation_policy: undocumented\n  failure_status: 401\n  note: >-\n    A single long-lived, unscoped credential carrying every permission its owner holds, including\n    delete on contacts, deals, tasks, events, tracks and tickets. There is no\
  \ way to issue a\n    read-only key, no way to scope a key to one object type, and no documented expiry or rotation\n    procedure. An agent handed this key holds the whole account. This is the dominant risk in\n    granting Agile CRM access to automation — record it in any onboarding.\nsso:\n  available: true\n  scope: application login only\n  guide: https://github.com/agilecrm/sso\n  note: >-\n    Agile CRM publishes an SSO setup guide for signing in to the application. It does not extend to\n    the REST API, which remains Basic-auth only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/authentication/agile-crm-authentication.yml
summary_line: http · 1 scheme
tags:
- CRM
- Sales Automation
- Marketing Automation
- Helpdesk
- Small Business
- Contact Management
---
