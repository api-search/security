---
anonymous_access: false
api_key_in: []
api_specs:
- filename: netwrix-openapi-generated.yml
  format: yaml
  label: Netwrix API
  slug: netwrix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netwrix/refs/heads/main/openapi/_ae-authored/netwrix-openapi-generated.yml
auth_types: []
description: Authentication for ServiceNow action
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Netwrix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Netwrix declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Netwrix
provider_slug: netwrix
scheme_count: 1
schemes:
- evidence: User Name/Password – Specify the credentials to access the ServiceNow account
  how_to_obtain: Enter the ServiceNow username and password in the Enterprise Auditor console’s global setting or in the action configuration
  name: ServiceNow
  type: http-basic
slug: netwrix-authentication
source_filename: netwrix-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.netwrix.com/docs/accessanalyzer/11_6/admin/action/servicenow/authentication
source_yaml: "generated: '2026-10-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.netwrix.com/docs/accessanalyzer/11_6/admin/action/servicenow/authentication\nsources:\n- https://docs.netwrix.com/docs/accessanalyzer/11_6/admin/action/servicenow/authentication\n- https://docs.netwrix.com/docs/accessanalyzer/11_6/solutions/databases/sql/configuration/sql_authentication\n- https://docs.netwrix.com/docs/accessanalyzer/11_6/tags/connection-profiles-and-credentials\n- https://docs.netwrix.com/docs/accessanalyzer/11_6/category/connection-profiles-and-credentials\ndescription: Authentication for ServiceNow action\nschemes:\n- type: http-basic\n  name: ServiceNow\n  evidence: User Name/Password – Specify the credentials to access the ServiceNow account\n  how_to_obtain: Enter the ServiceNow username and password in the Enterprise Auditor console’s global setting or in the action configuration\ndocs: https://docs.netwrix.com/docs/accessanalyzer/11_6/admin/action/servicenow/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netwrix/refs/heads/main/authentication/netwrix-authentication.yml
summary_line: 1 scheme
tags:
- Company
- DataSecurity
- Governance
- Compliance
- PrivilegedAccess
---
