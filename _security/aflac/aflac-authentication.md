---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aflac-claims-api-openapi.yml
  format: yaml
  label: aflac Claims API
  slug: aflac-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/openapi/aflac-claims-api-openapi.yml
- filename: aflac-eligibility-api-openapi.yml
  format: yaml
  label: aflac Eligibility API
  slug: aflac-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/openapi/aflac-eligibility-api-openapi.yml
- filename: aflac-enrollment-api-openapi.yml
  format: yaml
  label: aflac Enrollment API
  slug: aflac-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/openapi/aflac-enrollment-api-openapi.yml
- filename: aflac-groups-api-openapi.yml
  format: yaml
  label: aflac Groups API
  slug: aflac-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/openapi/aflac-groups-api-openapi.yml
- filename: aflac-policies-api-openapi.yml
  format: yaml
  label: aflac Policies API
  slug: aflac-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/openapi/aflac-policies-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Aflac Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Aflac secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Aflac
provider_slug: aflac
scheme_count: 1
schemes:
- client_authentication: HTTP Basic — client_id and client_secret sent as a Basic auth header
  credential_issuance: Internal ServiceNow request to the Security team ("oAuth / Ping Client Credential Request"). There is no self-serve or public signup path for AEC credentials.
  description: 'OAuth 2.0 client-credentials is the sole authentication method into the AEC API gateway. Aflac documents the full Postman setup: type OAuth 2.0, auth data added to request headers, header prefix Bearer, auto-refresh off, client authentication sent as a Basic auth header.'
  flows:
  - flow: clientCredentials
    scopes_published: false
    tokenUrl: null
    tokenUrl_note: 'NOT PUBLISHED ANONYMOUSLY. The Postman guide links an internal "Access Token URLs" page that the public content index does not carry. The value previously recorded here — https://auth.enterprise-connect.aflac.com/oauth/token — came from an API Evangelist-authored scaffold and is not a real host: DNS for auth.enterprise-connect.aflac.com returns NXDOMAIN (checked 2026-09-04). It has been removed rather than carried forward.'
  header: Authorization
  identity_provider: PingIdentity
  name: oauth2
  prefix: Bearer
  sources:
  - https://docs.enterprise-connect.aflac.com/docs/developer-guide/how-to-guides/how-to-make-a-request-to-aec-using-postman
  - https://docs.enterprise-connect.aflac.com/docs/developer-guide/how-to-guides/how-to-make-a-request-using-swagger
  type: oauth2
slug: aflac-authentication
source_filename: aflac-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: >-\n  https://docs.enterprise-connect.aflac.com/docs/developer-guide/how-to-guides/how-to-make-a-request-to-aec-using-postman\n  and .../how-to-make-a-request-using-swagger, .../how-to-deploy-a-new-service/things-to-set-up-prerequisite-tasks,\n  .../how-to-encrypt-and-decrypt, .../how-to-use-certificates — read from the Aflac Enterprise\n  Connect portal's public content index /assets/ng-doc/indexes.json (HTTP 200, 2026-09-04).\n  Upgrades the derived profile that was computed from openapi/_ae-authored/ scaffolds.\ndocs: https://docs.enterprise-connect.aflac.com/docs/developer-guide/how-to-guides/how-to-make-a-request-to-aec-using-postman\nprovider: aflac\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  exclusive: true\n  statement: >-\n    \"How can I make requests to AEC without using OAuth 2.0? Put simply - you cannot. OAuth 2.0 is\n    the only supported method for authenticating requests to AEC.\"\
  \nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: null\n    tokenUrl_note: >-\n      NOT PUBLISHED ANONYMOUSLY. The Postman guide links an internal \"Access Token URLs\" page that\n      the public content index does not carry. The value previously recorded here —\n      https://auth.enterprise-connect.aflac.com/oauth/token — came from an API Evangelist-authored\n      scaffold and is not a real host: DNS for auth.enterprise-connect.aflac.com returns NXDOMAIN\n      (checked 2026-09-04). It has been removed rather than carried forward.\n    scopes_published: false\n  header: Authorization\n  prefix: Bearer\n  client_authentication: HTTP Basic — client_id and client_secret sent as a Basic auth header\n  identity_provider: PingIdentity\n  credential_issuance: >-\n    Internal ServiceNow request to the Security team (\"oAuth / Ping Client Credential Request\").\n    There is no self-serve or public signup path for AEC credentials.\n  description:\
  \ >-\n    OAuth 2.0 client-credentials is the sole authentication method into the AEC API gateway. Aflac\n    documents the full Postman setup: type OAuth 2.0, auth data added to request headers, header\n    prefix Bearer, auto-refresh off, client authentication sent as a Basic auth header.\n  sources:\n  - https://docs.enterprise-connect.aflac.com/docs/developer-guide/how-to-guides/how-to-make-a-request-to-aec-using-postman\n  - https://docs.enterprise-connect.aflac.com/docs/developer-guide/how-to-guides/how-to-make-a-request-using-swagger\n\nadditional_headers:\n- header: aflac-openid-token\n  required: conditional\n  description: >-\n    Documented alongside the OAuth 2.0 header on the a-cipher aspect service — \"send POST request\n    to /a-cipher-1/v1/cipher-actions/protect with the appropriate OAuth 2.0 and aflac-openid-token\n    headers depending on environment\". A second, user-identity-bearing token distinct from the\n    machine client-credentials token.\n  source: https://docs.enterprise-connect.aflac.com/docs/developer-guide/how-to-guides/how-to-encrypt-and-decrypt\n\
  \ntransport_security:\n  mtls_inbound_required: false\n  note: >-\n    \"In AEC, you no longer need to use Mutual TLS (mTLS) to make requests to the running service in\n    AEC.\" mTLS remains in use for egress to third parties that enforce it and for legacy EIB 1.0\n    (Akana) systems; those certificates are managed through Venafi and injected into service\n    keystores automatically.\n  service_to_service: >-\n    Services inside AEC communicate directly across the service mesh without going back out through\n    the AWS API Gateway and without per-call certificates.\n\nportal_authentication:\n  provider: PingIdentity\n  federation: >-\n    Portal login in non-production uses an environment-suffixed identity — rmurphy@aflac.com becomes\n    rmurphy@aflacdev.com or rmurphy@aflacqa.com; a new PING profile may be required on first login.\n  saml_sso: Used for the Cloudsmith artifact registry (organization tag aflac-prod), not for the API.\n\ngate:\n  self_serve: false\n  public_signup:\
  \ false\n  note: >-\n    Every path to an AEC credential runs through an internal Aflac ServiceNow request. A member of\n    the public can read the platform's design rules in full but cannot obtain a token.\n\nanonymous_probe:\n  url: https://enterprise-connect.aflac.com/\n  status: 403\n  body: '{\"message\":\"Forbidden\"}'\n  checked: '2026-09-04'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/authentication/aflac-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Fortune 500
- Insurance
- Supplemental Insurance
- Employee Benefits
- Claims
- Enrollment
- Policy Administration
- Enterprise Integration
---
