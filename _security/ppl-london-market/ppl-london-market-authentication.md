---
api_key_in: []
api_specs:
- filename: ppl-london-market-placements.json
  format: json
  label: PPL Placements API
  slug: ppl-placements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-placements.json
- filename: ppl-london-market-submissions.json
  format: json
  label: PPL Submissions API
  slug: ppl-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-submissions.json
- filename: ppl-london-market-organisations.json
  format: json
  label: PPL Organisations API
  slug: ppl-organisations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-organisations.json
- filename: ppl-london-market-documents.json
  format: json
  label: PPL Documents API
  slug: ppl-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-documents.json
- filename: ppl-london-market-events.json
  format: json
  label: PPL Events API
  slug: ppl-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-events.json
auth_types:
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Ppl London Market Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- on-behalf-of
overview: PPL secures its APIs with oauth2 and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and on-behalf-of flow(s).
provider_name: PPL
provider_slug: ppl-london-market
scheme_count: 3
schemes:
- configuration:
    keys:
      CallbackPath: /signin-oidc
      ClientId: issued during onboarding
      ClientSecret: issued during onboarding
      Instance: https://login.microsoftonline.com/
      ResponseType: code id_token
      TenantId: environment specific (Sand, PreProd, Prod are separate tenanted environments)
    source: https://developer.pplnextgen.com/Get-Started/Authentication-Information
  description: 'Every business call is fronted by the LIMOSS API Gateway and must present a Microsoft Entra ID (Azure AD) JWT in the Authorization header as a bearer token. The Base API Standard states the JWT "must be signed by a Security Token Service (STS)" and must carry the claim "scp": "user_impersonation". Only identities that have been guested into the API Gateway Azure AD tenant for that environment can obtain a usable token.'
  flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize
    description: Browser sign-in for an application user. Configured in the portal's ASP.NET Core / MSAL sample as OpenID Connect with ResponseType "code id_token" and CallbackPath /signin-oidc, with the default authenticate scheme set to cookie authentication.
    flow: authorizationCode
    note: The token produced by the initial sign-in does NOT carry the scopes the gateway requires. The application must then request a second token directly from Azure AD on the user's behalf (on-behalf-of) before any API call will pass the gateway.
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  - description: 'OAuth 2.0 on-behalf-of exchange. Required when the initial token lacks the scope claim, and also when the downstream API validates the audience claim — "the gateway may also need to obtain an on-behalf-of token with the correct audience set". PPL documents the TTL rule explicitly: "Any token issued by the API Gateway must not have a TTL longer than that of the token which called it", with nbf set to the current time and exp matched to the original.'
    flow: onBehalfOf
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  - description: Service-account (headless) server-to-server token, used where no browser is involved. PPL notes that service-account tokens carry a dummy email claim.
    flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  header: 'Authorization: Bearer {JWT}'
  name: entraIdBearer
  optional_claims:
    amr: mfa
  required_claims:
    scp: user_impersonation
  type: oauth2
- description: 'Mutual HTTPS is mandatory. The Base API Standard requires an X.509 client certificate whose CN identifies the calling application. A DIFFERENT certificate must be registered for each API Gateway environment: "A different X.509 certificate should be used for each API Gateway (Sand, PreProd and Prod)." The portal''s sample loads the certificate from the Personal certificate store by thumbprint, gated on a UseCertificate configuration flag, with a one-hour sliding cache.'
  name: clientCertificate
  per_environment: true
  registration: https://admin.limoss.london/wp-content/uploads/2020/04/CS-Developers-On-Boarding-Guide-v1.1.pdf
  type: mutualTLS
- consumer_facing: false
  description: Documented as an alternative header scheme for non-token scenarios, carrying the user's email address. This is an internal/gateway construct, not a consumer credential — it does not replace the Entra ID bearer token or the client certificate for external consumers.
  in: header
  name: xAssertHeader
  parameter_name: X-Assert
  type: apiKey
slug: ppl-london-market-authentication
source_filename: ppl-london-market-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: openapi/ (5 OpenAPI 3.0.1 documents — none declares securitySchemes)\ndocs: https://developer.pplnextgen.com/Get-Started/Authentication-Information\nalso_documented_at:\n- https://developer.pplnextgen.com/Get-Started/Base-API-Standard\n- https://developer.pplnextgen.com/Get-Started/Registration-Onboarding\n- https://developer.pplnextgen.com/Get-Started/Reference-Architecture\nspec_gap: >-\n  None of the five published PPL OpenAPI documents declares components.securitySchemes and\n  none declares a security requirement. The entire auth contract lives in developer-portal\n  prose, not in the machine-readable artifacts. This profile is therefore SEARCHED from the\n  documentation, not derived from the specs. overlays/ppl-london-market-*-overlay.yaml carries\n  the securitySchemes PPL omits, as an OpenAPI Overlay over each original document.\nsummary:\n  types: [oauth2, mutualTLS]\n  api_keys: false\n  api_key_in: []\n  oauth2_flows:\
  \ [authorizationCode, clientCredentials, on-behalf-of]\n  identity_provider: Microsoft Entra ID (Azure AD)\n  gateway: LIMOSS API Gateway\n  self_serve: false\n  anonymous_endpoints: [/health]\nschemes:\n- name: entraIdBearer\n  type: oauth2\n  description: >-\n    Every business call is fronted by the LIMOSS API Gateway and must present a Microsoft Entra\n    ID (Azure AD) JWT in the Authorization header as a bearer token. The Base API Standard states\n    the JWT \"must be signed by a Security Token Service (STS)\" and must carry the claim\n    \"scp\": \"user_impersonation\". Only identities that have been guested into the API Gateway\n    Azure AD tenant for that environment can obtain a usable token.\n  header: 'Authorization: Bearer {JWT}'\n  required_claims:\n    scp: user_impersonation\n  optional_claims:\n    amr: mfa   # indicates the user completed multi-factor authentication\n  flows:\n  - flow: authorizationCode\n    description: >-\n      Browser sign-in for an application\
  \ user. Configured in the portal's ASP.NET Core / MSAL\n      sample as OpenID Connect with ResponseType \"code id_token\" and CallbackPath /signin-oidc,\n      with the default authenticate scheme set to cookie authentication.\n    authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n    note: >-\n      The token produced by the initial sign-in does NOT carry the scopes the gateway requires.\n      The application must then request a second token directly from Azure AD on the user's\n      behalf (on-behalf-of) before any API call will pass the gateway.\n  - flow: onBehalfOf\n    description: >-\n      OAuth 2.0 on-behalf-of exchange. Required when the initial token lacks the scope claim, and\n      also when the downstream API validates the audience claim — \"the gateway may also need to\n      obtain an on-behalf-of token with the correct audience set\". PPL documents the TTL\
  \ rule\n      explicitly: \"Any token issued by the API Gateway must not have a TTL longer than that of the\n      token which called it\", with nbf set to the current time and exp matched to the original.\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  - flow: clientCredentials\n    description: >-\n      Service-account (headless) server-to-server token, used where no browser is involved. PPL\n      notes that service-account tokens carry a dummy email claim.\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  configuration:\n    source: https://developer.pplnextgen.com/Get-Started/Authentication-Information\n    keys:\n      Instance: https://login.microsoftonline.com/\n      TenantId: environment specific (Sand, PreProd, Prod are separate tenanted environments)\n      ClientId: issued during onboarding\n      ClientSecret: issued during onboarding\n      CallbackPath: /signin-oidc\n      ResponseType: code id_token\n- name:\
  \ clientCertificate\n  type: mutualTLS\n  description: >-\n    Mutual HTTPS is mandatory. The Base API Standard requires an X.509 client certificate whose\n    CN identifies the calling application. A DIFFERENT certificate must be registered for each\n    API Gateway environment: \"A different X.509 certificate should be used for each API Gateway\n    (Sand, PreProd and Prod).\" The portal's sample loads the certificate from the Personal\n    certificate store by thumbprint, gated on a UseCertificate configuration flag, with a\n    one-hour sliding cache.\n  registration: https://admin.limoss.london/wp-content/uploads/2020/04/CS-Developers-On-Boarding-Guide-v1.1.pdf\n  per_environment: true\n- name: xAssertHeader\n  type: apiKey\n  in: header\n  parameter_name: X-Assert\n  description: >-\n    Documented as an alternative header scheme for non-token scenarios, carrying the user's email\n    address. This is an internal/gateway construct, not a consumer credential — it does not\n    replace\
  \ the Entra ID bearer token or the client certificate for external consumers.\n  consumer_facing: false\nrequired_call_headers:\n  note: >-\n    Derived from the parameters declared on every business operation across the five OpenAPI\n    documents. These are transmitted in addition to Authorization.\n  headers:\n  - name: X-Auth-Impersonated-User\n    required: true\n    scope: every business operation in all five APIs\n    description: The market user the call is being made on behalf of.\n  - name: X-Auth-Team\n    required: true\n    scope: every business operation except the Organisations broker/carrier organisation lookups\n    description: The broker or carrier team context for the call.\n  - name: X-Last-Modified\n    required: true\n    scope: every PUT (and Negotiation_Send_v1)\n    description: >-\n      Optimistic-concurrency precondition. PPL's implementation of the Base API Standard rule that\n      \"Resources must use optimistic concurrency control\"; the standard names\
  \ If-Match and\n      If-Unmodified-Since, the shipped APIs use the X-Last-Modified request header.\n  - name: X-Correlation-Id\n    required: false\n    scope: documented platform-wide for request tracing across the platform\nonboarding:\n  self_serve: false\n  gates:\n  - stage: 1\n    name: Developer Portal onboarding\n    action: Contact the PPL team\n    contact: PPLEnquiries@placingplatformlimited.com\n  - stage: 2\n    name: LIMOSS API Common Services subscription\n    action: >-\n      Register with the LIMOSS API Gateway and request \"Subscribe to PPL API\". New LIMOSS SSO\n      users go through the LIMOSS Service Desk; existing users use the LIMOSS Self-Service Portal.\n      The account is then guested into the Azure AD tenant of ONE environment — Sand, PreProd or\n      Prod — and each environment requires separate guesting.\n    urls:\n    - https://limoss.london/limoss-sso-sde-and-api-gateway\n    - https://limoss.london/contact\n    - https://customer.hornbill.com/limoss/\n\
  \  - stage: 3\n    name: Application and certificate registration\n    action: >-\n      Register the application in the Common Services Azure Active Directory and register an X.509\n      certificate, per environment.\n    guide: https://admin.limoss.london/wp-content/uploads/2020/04/CS-Developers-On-Boarding-Guide-v1.1.pdf\ndiscovery:\n  well_known: false\n  note: >-\n    No OpenID Connect discovery document and no RFC 8414 authorization-server metadata is served\n    on any PPL or LIMOSS gateway host — /.well-known/openid-configuration and\n    /.well-known/oauth-authorization-server return 404 on api.londonmarketgroup.co.uk,\n    sand-api.londonmarketgroup.co.uk, developer.pplnextgen.com, www.pplnextgen.com and\n    placingplatformlimited.com. Discovery happens through Microsoft's own tenant endpoints once a\n    TenantId has been issued during onboarding.\nrelated:\n  scopes: scopes/ppl-london-market-scopes.yml\n  conventions: conventions/ppl-london-market-conventions.yml\n  well_known:\
  \ well-known/ppl-london-market-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/authentication/ppl-london-market-authentication.yml
summary_line: oauth2/mutualTLS · 3 schemes
tags:
- Insurance
- United Kingdom
- London Market
- Lloyd's of London
- Reinsurance
- Commercial Insurance
- Broker
- Underwriting
- Placement
- Market Infrastructure
- ACORD
- Electronic Placing
---
