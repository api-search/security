---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Sepasoft Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sepasoft declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Sepasoft
provider_slug: sepasoft
scheme_count: 5
schemes:
- authorization: Optional "Required role(s)" field. If roles are listed the caller must hold at least one of them; multiple roles are comma separated. Blank means every role may call it.
  challenges:
    invalid_credentials: 403
    missing_credentials: 401 with a WWW-Authenticate header
  description: When "Basic" is selected on a RESTful endpoint resource, the endpoint requires HTTP BASIC authentication before the endpoint script executes.
  id: http-basic-provider
  identity_store: Ignition User Source (Gateway > Config > Security > Users, Roles > User Sources)
  role: provider
  scheme: basic
  source: https://docs.sepasoft.com/articles/user-manual/restful-endpoints
  surface: RESTful Endpoints and SOAP Endpoints served by the customer's Ignition Gateway
  type: http
- description: '"Redirect to SSL" option on a RESTful endpoint resource. When checked the endpoint is only reachable over SSL; a plaintext HTTP request is redirected to the Gateway SSL port.'
  id: transport-ssl-provider
  role: provider
  source: https://docs.sepasoft.com/articles/user-manual/restful-endpoints
  type: transport
- description: The RESTful Web Service Consumer supports the OAuth 2.0 Client Credentials grant for server-to-server calls out to third-party APIs. The Sepasoft manual's reference implementation is a self-hosted Keycloak realm; Sepasoft issues no tokens itself. Tokens are bearer JWTs minted by the operator's own authorization server.
  flow: clientCredentials
  id: oauth2-client-credentials-consumer
  role: consumer
  scopes_documented: false
  source: https://docs.sepasoft.com/articles/user-manual/configuring-oauth-client-credentials-for-restful-consumers
  token_endpoint: operator-supplied (no Sepasoft-hosted token endpoint exists)
  type: oauth2
- description: Outbound REST/SOAP consumer connections support Basic, Digest and NTLM authentication against the remote system, plus SSL encryption on all communications.
  id: http-basic-digest-ntlm-consumer
  role: consumer
  schemes:
  - basic
  - digest
  - ntlm
  source: https://www.sepasoft.com/products/web-services/
  type: http
- description: '"Enable SSL client authentication" on a consumer, with a Java KeyStore (JKS) keystore file + password for the client certificate and either the default `cacerts` truststore or an operator-supplied JKS truststore for verifying the server certificate.'
  id: mutual-tls-consumer
  role: consumer
  source: https://docs.sepasoft.com/articles/user-manual/consumers
  type: mutualTLS
slug: sepasoft-authentication
source_filename: sepasoft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://docs.sepasoft.com/articles/user-manual/restful-endpoints\ndocs:\n  - https://docs.sepasoft.com/articles/user-manual/restful-endpoints\n  - https://docs.sepasoft.com/articles/user-manual/soap-endpoints\n  - https://docs.sepasoft.com/articles/user-manual/consumers\n  - https://docs.sepasoft.com/articles/user-manual/configuring-oauth-client-credentials-for-restful-consumers\nprovider: Sepasoft\nproviderId: sepasoft\nsummary: >-\n  Sepasoft does not operate a hosted API. Its Web Services module turns the CUSTOMER'S\n  own Ignition Gateway into a REST/SOAP provider and consumer, so every auth decision\n  below is configured per deployment by the operator, not issued by Sepasoft. There are\n  no Sepasoft-issued API keys, no Sepasoft OAuth authorization server, and no Sepasoft\n  token endpoint. Documented as searched from the Sepasoft MES User Manual.\ndeployment_model: customer-hosted\nschemes:\n  - id: http-basic-provider\n\
  \    type: http\n    scheme: basic\n    role: provider\n    surface: RESTful Endpoints and SOAP Endpoints served by the customer's Ignition Gateway\n    description: >-\n      When \"Basic\" is selected on a RESTful endpoint resource, the endpoint requires HTTP\n      BASIC authentication before the endpoint script executes.\n    identity_store: Ignition User Source (Gateway > Config > Security > Users, Roles > User Sources)\n    authorization: >-\n      Optional \"Required role(s)\" field. If roles are listed the caller must hold at least\n      one of them; multiple roles are comma separated. Blank means every role may call it.\n    challenges:\n      missing_credentials: 401 with a WWW-Authenticate header\n      invalid_credentials: 403\n    source: https://docs.sepasoft.com/articles/user-manual/restful-endpoints\n  - id: transport-ssl-provider\n    type: transport\n    role: provider\n    description: >-\n      \"Redirect to SSL\" option on a RESTful endpoint resource. When checked\
  \ the endpoint is\n      only reachable over SSL; a plaintext HTTP request is redirected to the Gateway SSL port.\n    source: https://docs.sepasoft.com/articles/user-manual/restful-endpoints\n  - id: oauth2-client-credentials-consumer\n    type: oauth2\n    flow: clientCredentials\n    role: consumer\n    description: >-\n      The RESTful Web Service Consumer supports the OAuth 2.0 Client Credentials grant for\n      server-to-server calls out to third-party APIs. The Sepasoft manual's reference\n      implementation is a self-hosted Keycloak realm; Sepasoft issues no tokens itself.\n      Tokens are bearer JWTs minted by the operator's own authorization server.\n    token_endpoint: operator-supplied (no Sepasoft-hosted token endpoint exists)\n    scopes_documented: false\n    source: https://docs.sepasoft.com/articles/user-manual/configuring-oauth-client-credentials-for-restful-consumers\n  - id: http-basic-digest-ntlm-consumer\n    type: http\n    role: consumer\n    schemes:\n   \
  \   - basic\n      - digest\n      - ntlm\n    description: >-\n      Outbound REST/SOAP consumer connections support Basic, Digest and NTLM authentication\n      against the remote system, plus SSL encryption on all communications.\n    source: https://www.sepasoft.com/products/web-services/\n  - id: mutual-tls-consumer\n    type: mutualTLS\n    role: consumer\n    description: >-\n      \"Enable SSL client authentication\" on a consumer, with a Java KeyStore (JKS) keystore\n      file + password for the client certificate and either the default `cacerts` truststore\n      or an operator-supplied JKS truststore for verifying the server certificate.\n    source: https://docs.sepasoft.com/articles/user-manual/consumers\nnotes:\n  - >-\n    Because auth is configured per Ignition Gateway, there is no single documented base URL,\n    no Sepasoft-issued credential, and no published scope vocabulary. `scopes/` is therefore\n    deliberately absent rather than empty.\n  - >-\n    Endpoint scripts\
  \ are authored by the operator in Jython; a missing script for an HTTP\n    method returns 405 and a script syntax error returns 500 (see errors/).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sepasoft/refs/heads/main/authentication/sepasoft-authentication.yml
summary_line: 5 schemes
tags:
- Manufacturing
- Manufacturing Execution System
- Industrial Automation
- OEE
- Track and Trace
- Batch Processing
- Statistical Process Control
- ERP Integration
- ISA-95
- Ignition
---
