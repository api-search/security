---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Cyral Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Cyral secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Cyral
provider_slug: cyral
scheme_count: 2
schemes:
- credentials:
  - client_id
  - client_secret
  description: Machine-to-machine OAuth2 client-credentials grant against the customer's Cyral Control Plane. Returns an access_token used as a Bearer token for API calls. Control plane host is customer-specific (self-hosted / dedicated).
  flow: clientCredentials
  grant: client_credentials
  name: oauth2ClientCredentials
  token_url: https://<control-plane-host>:8000/v1/users/oidc/token
  type: oauth2
- bearer_format: JWT
  description: Access token from the client-credentials grant, sent as Authorization Bearer.
  name: bearerAuth
  scheme: bearer
  type: http
slug: cyral-authentication
source_filename: cyral-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  https://cyral.com/docs/api-ref/api-intro/ (archived) +\n  https://registry.terraform.io/providers/cyralinc/cyral/latest/docs\nnote: >-\n  Derived from documentation rather than a live OpenAPI spec (Cyral publishes no\n  public OpenAPI/Swagger; cyral.com now redirects to Varonis). The Cyral Control\n  Plane API uses OAuth2 client-credentials. A client obtains a token by POSTing a\n  clientId/clientSecret pair to the control plane token endpoint, then presents it\n  as a Bearer token. The Terraform provider is configured with control_plane,\n  client_id, and client_secret.\nsummary:\n  types: [oauth2, http]\n  oauth2_flows: [clientCredentials]\n  http_schemes: [bearer]\nschemes:\n  - name: oauth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_url: 'https://<control-plane-host>:8000/v1/users/oidc/token'\n    grant: client_credentials\n    credentials: [client_id, client_secret]\n    description:\
  \ >-\n      Machine-to-machine OAuth2 client-credentials grant against the customer's\n      Cyral Control Plane. Returns an access_token used as a Bearer token for API\n      calls. Control plane host is customer-specific (self-hosted / dedicated).\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    description: Access token from the client-credentials grant, sent as Authorization Bearer.\nidentity_providers:\n  - Okta (via terraform-okta-idp SCIM integration module)\n  - Generic SAML / OIDC IdP integrations supported by the control plane\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cyral/refs/heads/main/authentication/cyral-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Cybersecurity
- Data Security
- Database Activity Monitoring
- Data Governance
- Access Control
- Terraform
- SCIM
- OAuth
---
