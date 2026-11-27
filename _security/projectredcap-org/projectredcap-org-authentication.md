---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: REDCap (Vanderbilt) Authentication
name_suffix: Authentication
oauth_flows: []
overview: REDCap (Vanderbilt) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: REDCap (Vanderbilt)
provider_slug: projectredcap-org
scheme_count: 1
schemes:
- description: A REDCap API token sent as the token form field. Tokens are issued per installation. The token section of the core reference is behind a login.
  in: formData
  name: token
  type: apiKey
slug: projectredcap-org-authentication
source_filename: projectredcap-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://github.com/vanderbilt-redcap/external-module-framework-docs/blob/master/api.md\ndocs: https://github.com/vanderbilt-redcap/external-module-framework-docs/blob/master/api.md\nschemes:\n- name: token\n  type: apiKey\n  in: formData\n  description: A REDCap API token sent as the token form field. Tokens are issued per installation. The\n    token section of the core reference is behind a login.\nnote: OAuth2 appears only where REDCap acts as a client of an EHR FHIR service (CDIS), not as a way to\n  call the REDCap API.\n"
source_yaml_url: https://artifacts.apis.io/projectredcap-org/authentication/projectredcap-org-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Research
- Clinical Research
- Surveys
- Data Capture
- Healthcare
- Self-Hosted
---
