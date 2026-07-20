---
api_key_in: []
auth_types:
- session
description: ''
kind: authentication
layout: security
method: searched
name: Kace Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kace secures its APIs with session across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kace
provider_slug: kace
scheme_count: 1
schemes:
- login_body:
  - user name
  - password
  - organization (optional, for organization-enabled appliances)
  login_endpoint: POST /ams/shared/api/security/login
  name: kaceSessionLogin
  scheme: credentials-login
  sources:
  - docs
  type: session
slug: kace-authentication
source_filename: kace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://support.quest.com/technical-documents/kace-systems-management-appliance/15.0/api-reference-guide\ndocs: https://support.quest.com/technical-documents/kace-systems-management-appliance/15.0/api-reference-guide\nsummary:\n  types:\n  - session\n  note: >-\n    The KACE SMA REST API uses session-based authentication limited to authenticated KACE SMA\n    users. There are no OAuth2 flows or long-lived API keys documented; a client logs in with an\n    appliance user's credentials to establish an authenticated session against the customer-hosted\n    appliance host.\nschemes:\n- name: kaceSessionLogin\n  type: session\n  scheme: credentials-login\n  login_endpoint: POST /ams/shared/api/security/login\n  login_body:\n  - user name\n  - password\n  - organization (optional, for organization-enabled appliances)\n  sources:\n  - docs\nrequired_headers:\n- name: Accept\n  purpose: Select response format (application/json or application/xml)\n\
  - name: Content-Type\n  purpose: Declare request payload format (JSON or XML) on POST/PUT\n- name: x-kace-api-version\n  purpose: Select the API route version implementation (e.g. \"1\"); most recent used if unavailable\nnotes:\n- The API runs on the customer-hosted KACE SMA appliance; there is no shared public production host.\n- Access is limited to authenticated KACE SMA users; permissions follow the appliance user's role.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kace/refs/heads/main/authentication/kace-authentication.yml
summary_line: session · 1 scheme
tags:
- Company
- Endpoint Management
- Systems Management
- IT Asset Management
- Patch Management
- Service Desk
- Device Management
- Quest Software
---
