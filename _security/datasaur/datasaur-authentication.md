---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Datasaur Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Datasaur secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Datasaur
provider_slug: datasaur
scheme_count: 1
schemes:
- credentials:
  - client_id
  - client_secret
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  request_header: 'Authorization: Bearer <access token>'
  rfc: RFC 6749 section 4.4 (Client Credentials Grant)
  scopes: []
  scopes_note: Datasaur's client-credentials flow does not document a scope parameter; access is governed by the credential's team/workspace membership and role, not OAuth scopes.
  sources:
  - https://docs.datasaur.ai/api/credentials
  token_ttl_seconds: 3600
  token_type: bearer
  token_url: https://datasaur.ai/api/oauth/token
  type: oauth2
slug: datasaur-authentication
source_filename: datasaur-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.datasaur.ai/api/credentials\ndocs: https://docs.datasaur.ai/api/credentials\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  platform_sso: [SAML, SCIM]\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    grant_type: client_credentials\n    token_url: https://datasaur.ai/api/oauth/token\n    rfc: RFC 6749 section 4.4 (Client Credentials Grant)\n    credentials: [client_id, client_secret]\n    token_type: bearer\n    token_ttl_seconds: 3600\n    request_header: 'Authorization: Bearer <access token>'\n    scopes: []\n    scopes_note: >-\n      Datasaur's client-credentials flow does not document a scope parameter;\n      access is governed by the credential's team/workspace membership and role,\n      not OAuth scopes.\n    sources: [https://docs.datasaur.ai/api/credentials]\nplatform_authentication:\n  note: >-\n    Workspace/console access (distinct\
  \ from the API) supports enterprise SSO via\n    SAML and user/group provisioning via SCIM.\n  saml: https://docs.datasaur.ai/integrations/saml\n  scim: https://docs.datasaur.ai/integrations/scim\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datasaur/refs/heads/main/authentication/datasaur-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Enterprise Saas
- Data Labeling
- Artificial Intelligence
- Machine Learning
- Large Language Models
- NLP
- Data Annotation
- GraphQL
---
