---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: express-gateway-apps-api-openapi.yml
  format: yaml
  label: Express Gateway Apps API
  slug: express-gateway-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/express-gateway/refs/heads/main/openapi/express-gateway-apps-api-openapi.yml
- filename: express-gateway-credentials-api-openapi.yml
  format: yaml
  label: Express Gateway Credentials API
  slug: express-gateway-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/express-gateway/refs/heads/main/openapi/express-gateway-credentials-api-openapi.yml
- filename: express-gateway-scopes-api-openapi.yml
  format: yaml
  label: Express Gateway Scopes API
  slug: express-gateway-scopes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/express-gateway/refs/heads/main/openapi/express-gateway-scopes-api-openapi.yml
- filename: express-gateway-users-api-openapi.yml
  format: yaml
  label: Express Gateway Users API
  slug: express-gateway-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/express-gateway/refs/heads/main/openapi/express-gateway-users-api-openapi.yml
auth_types:
- apiKey
description: 'Authentication profile for the Express Gateway Admin API. The headline fact is that the Admin API ships with NO authentication: it binds to http://localhost:9876 and the reference states that public exposure "is not usually a great idea". Any auth on it is something the operator adds. The scheme below is the documented way to add it.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Express Gateway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Express Gateway secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Express Gateway
provider_slug: express-gateway
scheme_count: 1
schemes:
- description: 'The documented pattern is to expose the Admin API through Express Gateway itself: declare an apiEndpoint for the admin hostname, a serviceEndpoint pointing at http://localhost:9876, and a pipeline applying the key-auth policy followed by proxy. Callers then send "Authorization: apikey {keyId}:{keySecret}", where the pair comes from a key-auth credential issued to an admin user. The CLI reaches the same secured endpoint by setting `cli.url` in system.config.yml.'
  docs: https://www.express-gateway.io/docs/policies/key-authorization/
  format: apikey {keyId}:{keySecret}
  in: header
  name: KeyAuth
  parameter: Authorization
  sources:
  - https://www.express-gateway.io/docs/admin/
  - openapi/express-gateway-apps-api-openapi.yml
  - openapi/express-gateway-credentials-api-openapi.yml
  - openapi/express-gateway-scopes-api-openapi.yml
  - openapi/express-gateway-users-api-openapi.yml
  type: apiKey
slug: express-gateway-authentication
source_filename: express-gateway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://www.express-gateway.io/docs/admin/\ndocs: https://www.express-gateway.io/docs/admin/\nprovider: Express Gateway\nproviderId: express-gateway\ndescription: >-\n  Authentication profile for the Express Gateway Admin API. The headline fact is\n  that the Admin API ships with NO authentication: it binds to\n  http://localhost:9876 and the reference states that public exposure \"is not\n  usually a great idea\". Any auth on it is something the operator adds. The\n  scheme below is the documented way to add it.\ndefault_posture:\n  authenticated: false\n  binding: http://localhost:9876\n  detail: >-\n    Out of the box the Admin API is open on localhost. The reference's own\n    security guidance is to remove the `admin` section from gateway.config.yml to\n    disable it entirely, or to keep `hostname: localhost` so it is not reachable\n    off-host.\n  docs: https://www.express-gateway.io/docs/configuration/gateway.config.yml/admin/\n\
  summary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: KeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'apikey {keyId}:{keySecret}'\n  description: >-\n    The documented pattern is to expose the Admin API through Express Gateway\n    itself: declare an apiEndpoint for the admin hostname, a serviceEndpoint\n    pointing at http://localhost:9876, and a pipeline applying the key-auth policy\n    followed by proxy. Callers then send\n    \"Authorization: apikey {keyId}:{keySecret}\", where the pair comes from a\n    key-auth credential issued to an admin user. The CLI reaches the same secured\n    endpoint by setting `cli.url` in system.config.yml.\n  docs: https://www.express-gateway.io/docs/policies/key-authorization/\n  sources:\n  - https://www.express-gateway.io/docs/admin/\n  - openapi/express-gateway-apps-api-openapi.yml\n  - openapi/express-gateway-credentials-api-openapi.yml\n  - openapi/express-gateway-scopes-api-openapi.yml\n \
  \ - openapi/express-gateway-users-api-openapi.yml\ngateway_credential_types:\n  note: >-\n    Distinct from the Admin API's own auth: these are the credential types Express\n    Gateway issues to consumers of the APIs it fronts. Recorded here because the\n    Admin API is what creates them.\n  types:\n  - type: basic-auth\n    detail: Username and password. At most one per consumer.\n    docs: https://www.express-gateway.io/docs/policies/basic-authorization/\n  - type: key-auth\n    detail: keyId/keySecret pair. A consumer may hold many, which enables rotation.\n    docs: https://www.express-gateway.io/docs/policies/key-authorization/\n  - type: oauth2\n    detail: >-\n      Client secret or user password, RFC 6749. At most one per consumer. Express\n      Gateway acts as both authorization server and resource server, exposing\n      POST /oauth2/authorize and POST /oauth2/token.\n    docs: https://www.express-gateway.io/docs/policies/oauth2/\n  - type: jwt\n    detail: JWT issuing and\
  \ verification (RFC 7519), used to sign OAuth 2.0 tokens.\n    docs: https://www.express-gateway.io/docs/policies/jwt/\ndiscovery:\n  openid_configuration: false\n  oauth_authorization_server: false\n  detail: >-\n    Probed 2026-09-07 on www.express-gateway.io and express-gateway.io — both\n    /.well-known/openid-configuration and /.well-known/oauth-authorization-server\n    returned 404. Expected: the authorization server is the operator's own gateway\n    instance, not a host Express Gateway runs.\n  see: well-known/express-gateway-well-known.yml\nsee_also:\n- scopes/express-gateway-scopes.yml\n- conventions/express-gateway-conventions.yml\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/express-gateway/refs/heads/main/authentication/express-gateway-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Composition
- API Gateway
- BFF
- Open Source
- Microservices
- Authentication
- Node.js
- Reverse Proxy
---
