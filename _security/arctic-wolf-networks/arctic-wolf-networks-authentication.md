---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Arctic Wolf Networks Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Arctic Wolf Networks secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Arctic Wolf Networks
provider_slug: arctic-wolf-networks
scheme_count: 2
schemes:
- base_url: https://api-admin.cylance.com/public/v2
  description: The Aurora Multi-Tenant API authenticates a partner application with the OAuth 2.0 client-credentials grant. The Application ID (client id) and Application Secret (client secret) are presented as HTTP Basic Auth to the regional auth endpoint; the request body sets grant_type=client_credentials and scope=api. The response returns { access_token, expires_in, token_type }, and the access_token is then used as the Bearer token on all subsequent API calls.
  flow: clientCredentials
  name: AuroraMultiTenantOAuth
  scopes:
    api: Access to the Aurora Multi-Tenant / Endpoint Defense API surface.
  sources:
  - docs.arcticwolf.com
  token_url: https://api-admin.cylance.com/public/v2/{region_code}/auth
  token_url_example: https://api-admin.cylance.com/public/v2/us/auth
  type: oauth2
- description: Bearer access token (obtained from the client-credentials auth endpoint) presented on the Authorization header for all Aurora API resource calls.
  name: AuroraBearer
  scheme: bearer
  sources:
  - docs.arcticwolf.com
  type: http
slug: arctic-wolf-networks-authentication
source_filename: arctic-wolf-networks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.arcticwolf.com/en/developer-and-oem/aurora-multi-tenant-api/aurora-multi-tenant-api\ndocs: https://docs.arcticwolf.com/en/developer-and-oem/aurora-multi-tenant-api/aurora-multi-tenant-api/getting-started\nsummary:\n  types: [oauth2, http]\n  http_schemes: [bearer]\n  oauth2_flows: [clientCredentials]\nschemes:\n- name: AuroraMultiTenantOAuth\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    The Aurora Multi-Tenant API authenticates a partner application with the OAuth 2.0\n    client-credentials grant. The Application ID (client id) and Application Secret\n    (client secret) are presented as HTTP Basic Auth to the regional auth endpoint;\n    the request body sets grant_type=client_credentials and scope=api. The response\n    returns { access_token, expires_in, token_type }, and the access_token is then used\n    as the Bearer token on all subsequent API calls.\n  token_url: https://api-admin.cylance.com/public/v2/{region_code}/auth\n\
  \  token_url_example: https://api-admin.cylance.com/public/v2/us/auth\n  base_url: https://api-admin.cylance.com/public/v2\n  scopes:\n    api: Access to the Aurora Multi-Tenant / Endpoint Defense API surface.\n  sources: [docs.arcticwolf.com]\n- name: AuroraBearer\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer access token (obtained from the client-credentials auth endpoint) presented\n    on the Authorization header for all Aurora API resource calls.\n  sources: [docs.arcticwolf.com]\nnotes: >-\n  Arctic Wolf's Aurora Endpoint Defense / Multi-Tenant API is built on the Cylance\n  (BlackBerry) endpoint platform Arctic Wolf now operates; the auth and base hosts are\n  api-admin.cylance.com. Region codes select the login region (e.g. us).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arctic-wolf-networks/refs/heads/main/authentication/arctic-wolf-networks-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Cybersecurity
- Security Operations
- Managed Detection and Response
- Endpoint Security
- Threat Detection
- Incident Response
---
