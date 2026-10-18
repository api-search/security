---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cfengine-ai-api-openapi.yml
  format: yaml
  label: Cfengine AI API
  slug: cfengine-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfengine/refs/heads/main/openapi/cfengine-ai-api-openapi.yml
- filename: cfengine-build-api-openapi.yml
  format: yaml
  label: Cfengine Build API
  slug: cfengine-build-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfengine/refs/heads/main/openapi/cfengine-build-api-openapi.yml
- filename: cfengine-cfengine-api-api-openapi.yml
  format: yaml
  label: Cfengine Cfengine API
  slug: cfengine-cfengine-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfengine/refs/heads/main/openapi/cfengine-cfengine-api-api-openapi.yml
- filename: cfengine-cmdb-api-openapi.yml
  format: yaml
  label: Cfengine Cmdb API
  slug: cfengine-cmdb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfengine/refs/heads/main/openapi/cfengine-cmdb-api-openapi.yml
- filename: cfengine-hosts-api-openapi.yml
  format: yaml
  label: Cfengine Hosts API
  slug: cfengine-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfengine/refs/heads/main/openapi/cfengine-hosts-api-openapi.yml
- filename: cfengine-inventory-api-openapi.yml
  format: yaml
  label: Cfengine Inventory API
  slug: cfengine-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfengine/refs/heads/main/openapi/cfengine-inventory-api-openapi.yml
- filename: cfengine-rbac-api-openapi.yml
  format: yaml
  label: Cfengine Rbac API
  slug: cfengine-rbac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfengine/refs/heads/main/openapi/cfengine-rbac-api-openapi.yml
- filename: cfengine-role-api-openapi.yml
  format: yaml
  label: Cfengine Role API
  slug: cfengine-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfengine/refs/heads/main/openapi/cfengine-role-api-openapi.yml
- filename: cfengine-user-api-openapi.yml
  format: yaml
  label: Cfengine User API
  slug: cfengine-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfengine/refs/heads/main/openapi/cfengine-user-api-openapi.yml
auth_types: []
description: Authentication methods for CFEngine APIs
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Cfengine Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cfengine declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Cfengine
provider_slug: cfengine
scheme_count: 3
schemes:
- evidence: 'Headers: Authorization: api_token (string) Set token to access api. To get the token please look at - /var/cfengine/httpd/htdocs/ldap/config/settings.php'
  header: Authorization
  location: header
  name: api_token
  type: apiKey
- evidence: Basic authentication also requires this header each time it is used.
  header: Authorization
  location: header
  name: Basic
  type: http-basic
- evidence: 'Example request (curl): curl -X GET https://hub.cfengine.com/api/2fa/verification-needed --header ''Authorization: Bearer 627135e5a0b142cfdc738c38ad0c0067bc0960e5'''
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
slug: cfengine-authentication
source_filename: cfengine-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.cfengine.com/docs/lts/api/enterprise-api-ref/ldap-api/
source_yaml: "generated: '2026-10-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.cfengine.com/docs/lts/api/enterprise-api-ref/ldap-api/\nsources:\n- https://docs.cfengine.com/docs/lts/api/enterprise-api-ref/ldap-api/\n- https://docs.cfengine.com/docs/lts/api/enterprise-api-ref/two-factor-authentication/\n- https://docs.cfengine.com/docs/lts/web-ui/hub_administration/reset-admin-creds/\n- https://docs.cfengine.com/docs/lts/getting-started/\ndescription: Authentication methods for CFEngine APIs\nschemes:\n- type: apiKey\n  name: api_token\n  evidence: 'Headers: Authorization: api_token (string) Set token to access api. To get the token please look at - /var/cfengine/httpd/htdocs/ldap/config/settings.php'\n  location: header\n  header: Authorization\n- type: http-basic\n  name: Basic\n  evidence: Basic authentication also requires this header each time it is used.\n  location: header\n  header: Authorization\n- type: http-bearer\n  name: Bearer\n \
  \ evidence: 'Example request (curl): curl -X GET https://hub.cfengine.com/api/2fa/verification-needed --header ''Authorization: Bearer 627135e5a0b142cfdc738c38ad0c0067bc0960e5'''\n  location: header\n  header: Authorization\nnote: No OAuth flow details or scopes are documented on the provided pages.\ndocs: https://docs.cfengine.com/docs/lts/api/enterprise-api-ref/ldap-api/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cfengine/refs/heads/main/authentication/cfengine-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Automation
- Infrastructure
- Security
- Compliance
---
