---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Jama Software Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Jama Software secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Jama Software
provider_slug: jama-software
scheme_count: 2
schemes:
- description: HTTP Basic authentication (RFC 2617) using a Jama Connect username and password in the Authorization header. Available on all Jama Connect deployments.
  name: basicAuth
  scheme: basic
  sources:
  - https://dev.jamasoftware.com/api/
  type: http
- description: 'OAuth 2.0 client-credentials grant. Available on Jamacloud and self-hosted 8.62+. POST to /rest/oauth/token with grant_type=client_credentials using the client ID as HTTP Basic username and the client secret as password; the response returns an access_token and expires_in (default 3600s). Send the token as Authorization: Bearer {access_token} on subsequent calls.'
  flow: clientCredentials
  name: oauth2ClientCredentials
  sources:
  - https://dev.jamasoftware.com/api/
  tokenUrl: /rest/oauth/token
  type: oauth2
slug: jama-software-authentication
source_filename: jama-software-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://dev.jamasoftware.com/api/\ndocs: https://dev.jamasoftware.com/api/\nsummary:\n  types: [http, oauth2]\n  http_schemes: [basic]\n  oauth2_flows: [clientCredentials]\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic authentication (RFC 2617) using a Jama Connect username and\n      password in the Authorization header. Available on all Jama Connect\n      deployments.\n    sources: [https://dev.jamasoftware.com/api/]\n  - name: oauth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    tokenUrl: /rest/oauth/token\n    description: >-\n      OAuth 2.0 client-credentials grant. Available on Jamacloud and self-hosted\n      8.62+. POST to /rest/oauth/token with grant_type=client_credentials using\n      the client ID as HTTP Basic username and the client secret as password;\n      the response returns an access_token and expires_in (default 3600s). Send\n\
  \      the token as Authorization: Bearer {access_token} on subsequent calls.\n    sources: [https://dev.jamasoftware.com/api/]\nnotes:\n  - OAuth clients are provisioned by each user under their Jama Connect profile (API credentials).\n  - As of Jama Connect 9.4 the REST API is restricted to Creator-license users.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jama-software/refs/heads/main/authentication/jama-software-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Requirements Management
- Application Lifecycle Management
- Traceability
- Test Management
- Product Development
- Systems Engineering
- REST API
---
