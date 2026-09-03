---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: 'How a client authenticates to the Veradigm (formerly Allscripts) FHIR API. There is no OpenAPI document to derive securitySchemes from, so this profile is read from three live provider-served documents instead: the SMART App Launch configuration on the published sandbox base, the OpenID Connect discovery document on the authorization server it names as issuer, and the FHIR R4 CapabilityStatement, whose rest.security block declares SMART-on-FHIR and carries the SMART oauth-uris extension with the authorize and token endpoints. Veradigm implements the HL7 SMART Application Launch Framework Implementation Guide Release 2.0.0 and OpenID Connect Core 1.0.'
kind: authentication
layout: security
method: searched
name: Allscripts Healthcare Solutions Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Allscripts Healthcare Solutions secures its APIs with oauth2 and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Allscripts Healthcare Solutions
provider_slug: allscripts-healthcare-solutions
scheme_count: 4
schemes:
- audience: Patient and Provider FHIR applications
  authorizationUrl: https://fhir.fhirpoint.open.allscripts.com/fhirroute/authorizationV2/CP00101/connect/authorize
  flow: authorizationCode
  name: SMART on FHIR - standalone / EHR launch (authorization code)
  note: 'The capability statement is the discovery entry point: GET [FHIR base]/metadata returns the SMART oauth-uris extension carrying the authorize and token endpoints for that client environment. Redirect URLs (up to five) and launch URLs (up to three) are registered per application; desktop clients may register urn:ietf:wg:oauth:2.0:oob.'
  pkce:
  - plain
  - S256
  sources:
  - well-known/allscripts-healthcare-solutions-smart-configuration.json
  tokenUrl: https://fhir.fhirpoint.open.allscripts.com/fhirroute/authorizationV2/CP00101/connect/token
  type: oauth2
- audience: System FHIR applications only
  flow: clientCredentials
  name: SMART Backend Services (client credentials)
  note: Required for FHIR Bulk Data ($export). The application must be registered with App Type System and must publish a JWKS URL so Veradigm can validate the signed client assertion; Patient and User application types cannot make bulk data requests.
  sources:
  - well-known/allscripts-healthcare-solutions-smart-configuration.json
  - https://developer.veradigm.com/Fhir/BulkData
  tokenUrl: https://fhir.fhirpoint.open.allscripts.com/fhirroute/authorizationV2/CP00101/connect/token
  type: oauth2
- end_session_endpoint: https://fhirecho.fhirpoint.open.allscripts.com/pro/authorization/connect/endsession
  id_token_signing_alg_values_supported:
  - RS256
  introspection_endpoint: https://fhirecho.fhirpoint.open.allscripts.com/pro/authorization/connect/introspect
  issuer: https://fhirecho.fhirpoint.open.allscripts.com/pro/authorization
  jwks_uri: https://fhirecho.fhirpoint.open.allscripts.com/pro/authorization/.well-known/openid-configuration/jwks
  name: OpenID Connect
  openIdConnectUrl: https://fhirecho.fhirpoint.open.allscripts.com/pro/authorization/.well-known/openid-configuration
  revocation_endpoint: https://fhirecho.fhirpoint.open.allscripts.com/pro/authorization/connect/revocation
  sources:
  - well-known/allscripts-healthcare-solutions-openid-configuration.json
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - self_signed_tls_client_auth
  - tls_client_auth
  type: openIdConnect
  userinfo_endpoint: https://fhirecho.fhirpoint.open.allscripts.com/pro/authorization/connect/userinfo
- evidence: token_endpoint_auth_methods_supported includes tls_client_auth and self_signed_tls_client_auth; the discovery document publishes mtls_endpoint_aliases and tls_client_certificate_bound_access_tokens.
  name: Mutual TLS client authentication
  sources:
  - well-known/allscripts-healthcare-solutions-openid-configuration.json
  type: mutualTLS
slug: allscripts-healthcare-solutions-authentication
source_filename: allscripts-healthcare-solutions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: searched\nsource: https://fhir.fhirpoint.open.allscripts.com/fhirroute/fhir/CP00101/.well-known/smart-configuration,\n  https://fhirecho.fhirpoint.open.allscripts.com/pro/authorization/.well-known/openid-configuration, fhir/allscripts-healthcare-solutions-veradigm-fhir-r4-capabilitystatement.json\ndocs: https://developer.veradigm.com/Fhir/Introduction\ndescription: 'How a client authenticates to the Veradigm (formerly Allscripts) FHIR API. There is no OpenAPI\n  document to derive securitySchemes from, so this profile is read from three live provider-served documents\n  instead: the SMART App Launch configuration on the published sandbox base, the OpenID Connect discovery\n  document on the authorization server it names as issuer, and the FHIR R4 CapabilityStatement, whose\n  rest.security block declares SMART-on-FHIR and carries the SMART oauth-uris extension with the authorize\n  and token endpoints. Veradigm implements the HL7 SMART Application\
  \ Launch Framework Implementation Guide\n  Release 2.0.0 and OpenID Connect Core 1.0.'\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - refreshToken\n  pkce:\n  - S256\n  - plain\n  client_types:\n  - confidential (client_secret)\n  - confidential (private_key_jwt via developer-hosted JWKS)\n  - public\n  mutual_tls: true\n  dpop: true\n  pushed_authorization_requests: true\n  note: Credentials are not self-service. A developer registers on the Veradigm Connect portal, registers\n    a FHIR application (App Type Patient, Provider or System), and the portal issues a Client ID, Secret\n    and Secret Expiration Date. Before an application can reach a client organization the customer must\n    license it themselves in the separate client License Management Portal - the developer cannot do it\n    for them.\nschemes:\n- name: SMART on FHIR - standalone / EHR launch (authorization code)\n  type: oauth2\n\
  \  flow: authorizationCode\n  authorizationUrl: https://fhir.fhirpoint.open.allscripts.com/fhirroute/authorizationV2/CP00101/connect/authorize\n  tokenUrl: https://fhir.fhirpoint.open.allscripts.com/fhirroute/authorizationV2/CP00101/connect/token\n  pkce:\n  - plain\n  - S256\n  audience: Patient and Provider FHIR applications\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n  note: 'The capability statement is the discovery entry point: GET [FHIR base]/metadata returns the SMART\n    oauth-uris extension carrying the authorize and token endpoints for that client environment. Redirect\n    URLs (up to five) and launch URLs (up to three) are registered per application; desktop clients may\n    register urn:ietf:wg:oauth:2.0:oob.'\n- name: SMART Backend Services (client credentials)\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://fhir.fhirpoint.open.allscripts.com/fhirroute/authorizationV2/CP00101/connect/token\n  audience: System FHIR\
  \ applications only\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n  - https://developer.veradigm.com/Fhir/BulkData\n  note: Required for FHIR Bulk Data ($export). The application must be registered with App Type System\n    and must publish a JWKS URL so Veradigm can validate the signed client assertion; Patient and User\n    application types cannot make bulk data requests.\n- name: OpenID Connect\n  type: openIdConnect\n  openIdConnectUrl: https://fhirecho.fhirpoint.open.allscripts.com/pro/authorization/.well-known/openid-configuration\n  issuer: https://fhirecho.fhirpoint.open.allscripts.com/pro/authorization\n  jwks_uri: https://fhirecho.fhirpoint.open.allscripts.com/pro/authorization/.well-known/openid-configuration/jwks\n  userinfo_endpoint: https://fhirecho.fhirpoint.open.allscripts.com/pro/authorization/connect/userinfo\n  introspection_endpoint: https://fhirecho.fhirpoint.open.allscripts.com/pro/authorization/connect/introspect\n  revocation_endpoint:\
  \ https://fhirecho.fhirpoint.open.allscripts.com/pro/authorization/connect/revocation\n  end_session_endpoint: https://fhirecho.fhirpoint.open.allscripts.com/pro/authorization/connect/endsession\n  id_token_signing_alg_values_supported:\n  - RS256\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - self_signed_tls_client_auth\n  - tls_client_auth\n  sources:\n  - well-known/allscripts-healthcare-solutions-openid-configuration.json\n- name: Mutual TLS client authentication\n  type: mutualTLS\n  evidence: token_endpoint_auth_methods_supported includes tls_client_auth and self_signed_tls_client_auth;\n    the discovery document publishes mtls_endpoint_aliases and tls_client_certificate_bound_access_tokens.\n  sources:\n  - well-known/allscripts-healthcare-solutions-openid-configuration.json\ntoken_lifetime:\n  documented: false\n  note: Veradigm states token validity is configured per client in the Veradigm License Management Portal,\n    so no\
  \ fixed TTL is published.\n  source: https://developer.veradigm.com/Fhir/Introduction\ncapabilities_advertised:\n- launch-ehr\n- launch-standalone\n- client-public\n- client-confidential-symmetric\n- context-ehr-patient\n- context-ehr-encounter\n- context-standalone-patient\n- context-standalone-encounter\n- context-passthrough-banner\n- context-passthrough-style\n- context-banner\n- context-style\n- sso-openid-connect\n- permission-offline\n- permission-patient\n- permission-user\n- client-confidential-asymmetric\n- authorize-post\n- permission-v1\n- permission-v2\ngated:\n  unity_api: The proprietary bidirectional Unity API - the only Veradigm surface that can write patient\n    demographic, appointment or financial data - is not documented publicly. Its authentication model\n    could not be observed; access requires a paid Veradigm Connect Integrator subscription.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allscripts-healthcare-solutions/refs/heads/main/authentication/allscripts-healthcare-solutions-authentication.yml
summary_line: oauth2/openIdConnect · 4 schemes
tags:
- Healthcare IT
- EHR
- Clinical
- FHIR
- HL7
- SMART on FHIR
- USCDI
- Interoperability
- Patient Access
- 21st Century Cures
- Veradigm
---
