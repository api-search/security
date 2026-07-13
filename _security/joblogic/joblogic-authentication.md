---
api_key_in: []
api_specs:
- filename: joblogic-openapi.yml
  format: yaml
  label: Joblogic Customers API
  slug: joblogic-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/joblogic/refs/heads/main/openapi/joblogic-openapi.yml
- filename: joblogic-openapi.yml
  format: yaml
  label: Joblogic Contacts API
  slug: joblogic-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/joblogic/refs/heads/main/openapi/joblogic-openapi.yml
- filename: joblogic-openapi.yml
  format: yaml
  label: Joblogic Sites API
  slug: joblogic-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/joblogic/refs/heads/main/openapi/joblogic-openapi.yml
- filename: joblogic-openapi.yml
  format: yaml
  label: Joblogic Assets API
  slug: joblogic-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/joblogic/refs/heads/main/openapi/joblogic-openapi.yml
- filename: joblogic-openapi.yml
  format: yaml
  label: Joblogic Jobs API
  slug: joblogic-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/joblogic/refs/heads/main/openapi/joblogic-openapi.yml
- filename: joblogic-openapi.yml
  format: yaml
  label: Joblogic Visits API
  slug: joblogic-visits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/joblogic/refs/heads/main/openapi/joblogic-openapi.yml
- filename: joblogic-openapi.yml
  format: yaml
  label: Joblogic Engineers API
  slug: joblogic-engineers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/joblogic/refs/heads/main/openapi/joblogic-openapi.yml
- filename: joblogic-openapi.yml
  format: yaml
  label: Joblogic Quotes API
  slug: joblogic-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/joblogic/refs/heads/main/openapi/joblogic-openapi.yml
- filename: joblogic-openapi.yml
  format: yaml
  label: Joblogic Invoices API
  slug: joblogic-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/joblogic/refs/heads/main/openapi/joblogic-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Joblogic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Joblogic secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Joblogic
provider_slug: joblogic
scheme_count: 1
schemes:
- description: 'OAuth2 client-credentials grant against the Joblogic IdentityServer. A caller POSTs client_id, client_secret, grant_type=client_credentials, and the issued scope (as application/x-www-form-urlencoded) to the token endpoint, then passes the returned access token as `Authorization: Bearer <access_token>` on every API request. Access tokens expire after one hour; expired or missing tokens return 401 Unauthorized. The confirmed UAT token endpoint is https://uatidentityserver.joblogic.com/connect/token; the production IdentityServer token endpoint, the Client ID, Client Secret, Tenant ID, and scope are all provisioned to the caller by Joblogic during onboarding, and the caller''s public IP addresses must be allowlisted behind Joblogic''s firewall before access is granted.'
  flow: clientCredentials
  grantType: client_credentials
  name: oauth2ClientCredentials
  sources:
  - openapi/joblogic-openapi.yml
  - https://apidocs.joblogic.com/
  - https://support.joblogic.com/docs/api-access
  tokenUrl: https://uatidentityserver.joblogic.com/connect/token
  type: oauth2
slug: joblogic-authentication
source_filename: joblogic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/joblogic-openapi.yml\nsummary:\n  types:\n  - oauth2\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://uatidentityserver.joblogic.com/connect/token\n  grantType: client_credentials\n  description: >-\n    OAuth2 client-credentials grant against the Joblogic IdentityServer. A\n    caller POSTs client_id, client_secret, grant_type=client_credentials, and\n    the issued scope (as application/x-www-form-urlencoded) to the token\n    endpoint, then passes the returned access token as `Authorization: Bearer\n    <access_token>` on every API request. Access tokens expire after one hour;\n    expired or missing tokens return 401 Unauthorized. The confirmed UAT token\n    endpoint is https://uatidentityserver.joblogic.com/connect/token; the\n    production IdentityServer token endpoint, the Client ID, Client Secret,\n    Tenant ID, and scope are all provisioned to the\
  \ caller by Joblogic during\n    onboarding, and the caller's public IP addresses must be allowlisted behind\n    Joblogic's firewall before access is granted.\n  sources:\n  - openapi/joblogic-openapi.yml\n  - https://apidocs.joblogic.com/\n  - https://support.joblogic.com/docs/api-access\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/joblogic/refs/heads/main/authentication/joblogic-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Field Service Management
- Job Management
- Scheduling
- Maintenance
- Workforce
- Mobile Workforce
- Trades
- CRM
- SaaS
---
