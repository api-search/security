---
anonymous_access: true
api_key_in:
- header
api_specs:
- filename: f5-mgmt-api-openapi.yml
  format: yaml
  label: F5 BIG-IP iControl REST (Mgmt)
  slug: f5-mgmt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/openapi/f5-mgmt-api-openapi.yml
- filename: f5-nginx-plus-api-openapi.yml
  format: yaml
  label: NGINX Plus REST API
  slug: f5-nginx-plus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/openapi/f5-nginx-plus-api-openapi.yml
- filename: f5-big-ip-as3-openapi.yml
  format: yaml
  label: F5 BIG-IP AS3 (Application Services 3 Extension)
  slug: f5-big-ip-as3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/openapi/f5-big-ip-as3-openapi.yml
- filename: f5-big-ip-fast-openapi.yml
  format: yaml
  label: F5 BIG-IP Application Services Templates (FAST)
  slug: f5-big-ip-fast
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/openapi/f5-big-ip-fast-openapi.yml
- filename: f5-big-ip-declarative-onboarding-openapi.yml
  format: yaml
  label: F5 BIG-IP Declarative Onboarding
  slug: f5-big-ip-declarative-onboarding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/openapi/f5-big-ip-declarative-onboarding-openapi.yml
- filename: f5-nginx-plus-api-openapi.yml
  format: yaml
  label: F5 NGINX Plus API
  slug: f5-nginx-plus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/openapi/f5-nginx-plus-api-openapi.yml
- filename: f5-nodes-api-openapi.yml
  format: yaml
  label: F5 Networks Nodes API
  slug: f5-networks-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/openapi/f5-nodes-api-openapi.yml
- filename: f5-pool-members-api-openapi.yml
  format: yaml
  label: F5 Networks Pool Members API
  slug: f5-networks-pool-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/openapi/f5-pool-members-api-openapi.yml
- filename: f5-pools-api-openapi.yml
  format: yaml
  label: F5 Networks Pools API
  slug: f5-networks-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/openapi/f5-pools-api-openapi.yml
- filename: f5-profiles-api-openapi.yml
  format: yaml
  label: F5 Networks Profiles API
  slug: f5-networks-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/openapi/f5-profiles-api-openapi.yml
- filename: f5-virtual-servers-api-openapi.yml
  format: yaml
  label: F5 Networks Virtual Servers API
  slug: f5-networks-virtual-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/openapi/f5-virtual-servers-api-openapi.yml
auth_types:
- http
- apiKey
- mutualTLS
- none
description: 'F5 has no single authentication story because it has no single API. There is no F5 account, no F5-issued API key, and no OAuth anywhere in the product estate. What there is: device credentials for the BIG-IP APIs, an nginx.conf policy decision for the NGINX Plus API, and a tenant-scoped token or client certificate for the two hosted surfaces. An integrator needs to know which of the three they are in before writing a line of code.'
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: F5 Authentication
name_suffix: Authentication
oauth_flows: []
overview: F5 secures its APIs with http, apiKey, mutualTLS, and none across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: F5
provider_slug: f5
scheme_count: 5
schemes:
- applies_to:
  - F5 BIG-IP iControl REST
  - F5 BIG-IP AS3
  - F5 BIG-IP FAST
  - F5 BIG-IP Declarative Onboarding
  description: HTTP Basic over TLS using a BIG-IP administrative user. Works on every /mgmt/ endpoint and is the simplest path for a script. The credential is a device account, not an F5 cloud account.
  name: Basic
  scheme: basic
  sources:
  - openapi/f5-mgmt-api-openapi.yml
  - https://clouddocs.f5.com/api/icontrol-rest/
  type: http
- applies_to:
  - F5 BIG-IP iControl REST
  - F5 BIG-IP AS3
  - F5 BIG-IP FAST
  - F5 BIG-IP Declarative Onboarding
  description: A device-issued token exchanged for username/password at /mgmt/shared/authn/login. Default timeout is 1200 seconds; the token resource can be PATCHed to extend it. Preferred over Basic for anything long-running because it avoids replaying the password on every call.
  in: header
  name: Token
  parameter: X-F5-Auth-Token
  sources:
  - openapi/f5-mgmt-api-openapi.yml
  - https://clouddocs.f5.com/api/icontrol-rest/
  token_endpoint: POST /mgmt/shared/authn/login
  token_request:
    loginProviderName: tmos
    password: string
    username: string
  ttl_seconds: 1200
  type: apiKey
- applies_to:
  - F5 Distributed Cloud
  - NGINX One Console
  description: Tenant-scoped API token generated in the F5 Distributed Cloud / NGINX One console. Note the non-standard scheme name — it is "APIToken", not "Bearer", and a client that assumes Bearer will fail authentication.
  format: 'Authorization: APIToken <token-value>'
  in: header
  name: APIToken
  parameter: Authorization
  sources:
  - https://docs.nginx.com/nginx-one-console/api/authentication/
  type: apiKey
- applies_to:
  - F5 Distributed Cloud
  - NGINX One Console
  description: A PKCS#12 bundle (key + certificate) downloaded from the tenant console, with the passphrase supplied separately. This is the default for vesctl, which reads it from $HOME/.vesconfig as the `p12-bundle` key and takes the password from the VES_P12_PASSWORD environment variable. Certificate-based auth is awkward for ephemeral agent and CI environments — plan the secret handling before choosing it over the API token.
  name: P12ClientCertificate
  sources:
  - https://docs.nginx.com/nginx-one-console/api/authentication/
  - https://gitlab.com/volterra.io/vesctl/-/raw/main/README.md
  type: mutualTLS
- applies_to:
  - NGINX Plus REST API
  description: 'The NGINX Plus REST API declares no securityScheme, and that is deliberate rather than an omission in the contract. Access control is a configuration concern enforced in the nginx.conf location that serves the API — allow/deny, auth_basic, or client certificates, whatever the operator chose. Write access is separately gated by the `api write=on;` directive; without it every mutation returns 405 with internal error code MethodDisabled. The practical consequence: an NGINX Plus API is unauthenticated and read-only until an operator decides otherwise, and an agent cannot discover which of those it is facing except by trying.'
  name: NoneDeclared
  sources:
  - openapi/f5-nginx-plus-api-openapi.yml
  - https://nginx.org/en/docs/http/ngx_http_api_module.html
  type: none
slug: f5-authentication
source_filename: f5-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: >-\n  Derived from the securitySchemes and prose of the five contracts in openapi/, then upgraded from\n  the provider's own documentation: https://docs.nginx.com/nginx-one-console/api/authentication/\n  (200), https://nginx.org/en/docs/http/ngx_http_api_module.html (200),\n  https://clouddocs.f5.com/api/icontrol-rest/ (200), the vesctl README at\n  https://gitlab.com/volterra.io/vesctl/-/raw/main/README.md (200), and the OIDC discovery document\n  saved to well-known/f5-my-openid-configuration.json. All probed 2026-09-07.\ndocs:\n  - https://docs.nginx.com/nginx-one-console/api/authentication/\n  - https://clouddocs.f5.com/api/icontrol-rest/\n  - https://nginx.org/en/docs/http/ngx_http_api_module.html\ndescription: >-\n  F5 has no single authentication story because it has no single API. There is no F5 account, no\n  F5-issued API key, and no OAuth anywhere in the product estate. What there is: device credentials\n  for the\
  \ BIG-IP APIs, an nginx.conf policy decision for the NGINX Plus API, and a tenant-scoped\n  token or client certificate for the two hosted surfaces. An integrator needs to know which of the\n  three they are in before writing a line of code.\nsummary:\n  types:\n    - http\n    - apiKey\n    - mutualTLS\n    - none\n  api_key_in:\n    - header\n  oauth2: false\n  oauth2_note: >-\n    No securityScheme of type oauth2 or openIdConnect appears in any published F5 contract. The one\n    OIDC surface F5 serves (my.f5.com) authorizes the Salesforce-backed support portal, not any\n    product API — see conformance/f5-conformance.yml.\nschemes:\n  - name: Basic\n    type: http\n    scheme: basic\n    applies_to:\n      - F5 BIG-IP iControl REST\n      - F5 BIG-IP AS3\n      - F5 BIG-IP FAST\n      - F5 BIG-IP Declarative Onboarding\n    description: >-\n      HTTP Basic over TLS using a BIG-IP administrative user. Works on every /mgmt/ endpoint and is\n      the simplest path for a script. The\
  \ credential is a device account, not an F5 cloud account.\n    sources:\n      - openapi/f5-mgmt-api-openapi.yml\n      - https://clouddocs.f5.com/api/icontrol-rest/\n  - name: Token\n    type: apiKey\n    in: header\n    parameter: X-F5-Auth-Token\n    applies_to:\n      - F5 BIG-IP iControl REST\n      - F5 BIG-IP AS3\n      - F5 BIG-IP FAST\n      - F5 BIG-IP Declarative Onboarding\n    token_endpoint: POST /mgmt/shared/authn/login\n    token_request:\n      username: string\n      password: string\n      loginProviderName: tmos\n    ttl_seconds: 1200\n    description: >-\n      A device-issued token exchanged for username/password at /mgmt/shared/authn/login. Default\n      timeout is 1200 seconds; the token resource can be PATCHed to extend it. Preferred over Basic\n      for anything long-running because it avoids replaying the password on every call.\n    sources:\n      - openapi/f5-mgmt-api-openapi.yml\n      - https://clouddocs.f5.com/api/icontrol-rest/\n  - name: APIToken\n\
  \    type: apiKey\n    in: header\n    parameter: Authorization\n    format: 'Authorization: APIToken <token-value>'\n    applies_to:\n      - F5 Distributed Cloud\n      - NGINX One Console\n    description: >-\n      Tenant-scoped API token generated in the F5 Distributed Cloud / NGINX One console. Note the\n      non-standard scheme name — it is \"APIToken\", not \"Bearer\", and a client that assumes Bearer\n      will fail authentication.\n    sources:\n      - https://docs.nginx.com/nginx-one-console/api/authentication/\n  - name: P12ClientCertificate\n    type: mutualTLS\n    applies_to:\n      - F5 Distributed Cloud\n      - NGINX One Console\n    description: >-\n      A PKCS#12 bundle (key + certificate) downloaded from the tenant console, with the passphrase\n      supplied separately. This is the default for vesctl, which reads it from $HOME/.vesconfig as\n      the `p12-bundle` key and takes the password from the VES_P12_PASSWORD environment variable.\n      Certificate-based\
  \ auth is awkward for ephemeral agent and CI environments — plan the secret\n      handling before choosing it over the API token.\n    sources:\n      - https://docs.nginx.com/nginx-one-console/api/authentication/\n      - https://gitlab.com/volterra.io/vesctl/-/raw/main/README.md\n  - name: NoneDeclared\n    type: none\n    applies_to:\n      - NGINX Plus REST API\n    description: >-\n      The NGINX Plus REST API declares no securityScheme, and that is deliberate rather than an\n      omission in the contract. Access control is a configuration concern enforced in the nginx.conf\n      location that serves the API — allow/deny, auth_basic, or client certificates, whatever the\n      operator chose. Write access is separately gated by the `api write=on;` directive; without it\n      every mutation returns 405 with internal error code MethodDisabled.\n      The practical consequence: an NGINX Plus API is unauthenticated and read-only until an\n      operator decides otherwise, and an\
  \ agent cannot discover which of those it is facing except\n      by trying.\n    sources:\n      - openapi/f5-nginx-plus-api-openapi.yml\n      - https://nginx.org/en/docs/http/ngx_http_api_module.html\nbase_urls:\n  - api: F5 BIG-IP iControl REST / AS3 / FAST / DO\n    base: https://{bigip}/mgmt/\n    hosted_by: customer\n  - api: NGINX Plus REST API\n    base: https://{nginx-host}/api/{version}\n    hosted_by: customer\n  - api: F5 Distributed Cloud\n    base: https://{tenant}.console.ves.volterra.io/api\n    hosted_by: F5\n  - api: NGINX One Console\n    base: https://{tenant}.console.ves.volterra.io/api/nginx/one/namespaces/{namespace}/{kind}\n    hosted_by: F5\nportal_identity:\n  host: my.f5.com\n  protocol: OpenID Connect\n  discovery: well-known/f5-my-openid-configuration.json\n  issuer: https://my.f5.com\n  note: >-\n    F5's customer support portal serves a complete OIDC discovery document. It runs on Salesforce\n    Experience Cloud — the scopes_supported list is the Salesforce\
  \ platform vocabulary — and it\n    authorizes the portal, not BIG-IP, NGINX or Distributed Cloud APIs. Recorded here so it is not\n    mistaken for a product API auth surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/authentication/f5-authentication.yml
summary_line: http/apiKey/mutualTLS/none · 5 schemes
tags:
- Application
- Security
- Load Balancing
- API Gateway
- WAF
---
