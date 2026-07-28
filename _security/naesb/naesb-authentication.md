---
api_key_in: []
auth_types:
- mutualTLS
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Naesb Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: NAESB secures its APIs with mutualTLS and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: NAESB
provider_slug: naesb
scheme_count: 2
schemes:
- additional_requirement: A paid EIR registration and annual subscription is required in addition to the certificate. The annual subscription fee rose to $275 effective 2025-10-01.
  api: naesb:naesb-eir-webregistry
  authorized_ca_list: https://www.naesb.org/pdf4/ac_authorities_2023.pdf
  issuer_model: X.509 certificates issued by NAESB-Authorized Certification Authorities (ACAs) accredited under NAESB WEQ-012 Public Key Infrastructure. The registry itself publishes the ACA roster through the DownloadACA and DownloadPKICA operations, whose ACAStruct carries PKICAName, CertificateURL and CertificateType (ROOT | INTERMEDIATE | ISSUER).
  minimum_tls: TLSv1.2
  minimum_tls_source: https://www.naesb.org/pdf4/registry_required_browser_settings_tls-v1.2_0320.pdf
  name: NAESB EIR client certificate
  sources:
  - wsdl/naesb-eir-webregistry.wsdl
  transport: https
  type: mutualTLS
  verified_behavior:
    date: '2026-07-27'
    finding: The service is reachable and answers anonymously with a well-formed SOAP body, but every operation is refused without a registered client certificate. The WSDL itself is served to anonymous callers; only the data behind it is gated.
    http_status: 200
    probe: Anonymous SOAP POST of DownloadRegistryVersion to the production endpoint, no client certificate presented.
    response_error_code_desc: Please present a valid certificate that is associated with a NAESB EIR user
    response_return_code: 1
    response_return_code_desc: FAILURE
- api: naesb:naesb-espi-green-button
  flows:
  - flow: authorizationCode
    note: The v4.0 schema encodes the endpoints as data rather than fixing them, because every Data Custodian runs its own authorization server. ApplicationInformation carries authorizationServerUri, authorizationServerAuthorizationEndpoint, authorizationServerTokenEndpoint and authorizationServerRegistrationEndpoint; GrantType and TokenEndPointMethod select the flow and client authentication method.
  name: ESPI OAuth 2.0 (authored by NAESB, implemented by each Data Custodian)
  operated_by: each utility Data Custodian, not NAESB
  schema_elements:
  - authorizationServerUri
  - authorizationServerAuthorizationEndpoint
  - authorizationServerTokenEndpoint
  - authorizationServerRegistrationEndpoint
  - GrantType
  - TokenEndPointMethod
  - scope
  - OAuthError
  scopes_note: The schema declares a `scope` element and an Authorization resource, but the scope string grammar and its permitted values live in the copyright-protected REQ.21 Model Business Practices narrative, which NAESB paywalls. No scope vocabulary is published openly, so no scopes/ artifact is emitted for this provider rather than guessing one.
  sources:
  - schemas/naesb-espi_v4.xsd
  type: oauth2
slug: naesb-authentication
source_filename: naesb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  wsdl/naesb-eir-webregistry.wsdl (harvested live), a verified anonymous SOAP call to the\n  production EIR webRegistry endpoint on 2026-07-27, the OATI webRegistry Technical Guide\n  v6.1, the NAESB Authorized Certification Authority list, and the ESPI v4.0 XML schema.\ndocs: https://www.naesb.org/pdf4/eir_webregistry_technical_guide_v6.1_1018.pdf\nsummary:\n  types:\n  - mutualTLS\n  - oauth2\n  note: >-\n    NAESB has two entirely separate authentication stories and they must not be conflated.\n    The one API NAESB itself operates — the EIR webRegistry — is protected by mutual TLS\n    with X.509 client certificates issued by NAESB-Authorized Certification Authorities.\n    The OAuth 2.0 model below is NOT NAESB authentication: it is the authorization model\n    that the REQ.21 ESPI (Green Button) standard requires each utility Data Custodian to\n    implement at its own endpoint. NAESB authors that model; it operates\
  \ no ESPI endpoint.\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: NAESB EIR client certificate\n  api: naesb:naesb-eir-webregistry\n  type: mutualTLS\n  transport: https\n  sources:\n  - wsdl/naesb-eir-webregistry.wsdl\n  issuer_model: >-\n    X.509 certificates issued by NAESB-Authorized Certification Authorities (ACAs) accredited\n    under NAESB WEQ-012 Public Key Infrastructure. The registry itself publishes the ACA\n    roster through the DownloadACA and DownloadPKICA operations, whose ACAStruct carries\n    PKICAName, CertificateURL and CertificateType (ROOT | INTERMEDIATE | ISSUER).\n  authorized_ca_list: https://www.naesb.org/pdf4/ac_authorities_2023.pdf\n  minimum_tls: TLSv1.2\n  minimum_tls_source: https://www.naesb.org/pdf4/registry_required_browser_settings_tls-v1.2_0320.pdf\n  additional_requirement: >-\n    A paid EIR registration and annual subscription is required in addition to the certificate.\n    The annual subscription fee rose to $275\
  \ effective 2025-10-01.\n  verified_behavior:\n    date: '2026-07-27'\n    probe: >-\n      Anonymous SOAP POST of DownloadRegistryVersion to the production endpoint, no client\n      certificate presented.\n    http_status: 200\n    response_return_code: 1\n    response_return_code_desc: FAILURE\n    response_error_code_desc: Please present a valid certificate that is associated with a NAESB EIR user\n    finding: >-\n      The service is reachable and answers anonymously with a well-formed SOAP body, but every\n      operation is refused without a registered client certificate. The WSDL itself is served\n      to anonymous callers; only the data behind it is gated.\n- name: ESPI OAuth 2.0 (authored by NAESB, implemented by each Data Custodian)\n  api: naesb:naesb-espi-green-button\n  type: oauth2\n  operated_by: each utility Data Custodian, not NAESB\n  sources:\n  - schemas/naesb-espi_v4.xsd\n  flows:\n  - flow: authorizationCode\n    note: >-\n      The v4.0 schema encodes the endpoints\
  \ as data rather than fixing them, because every\n      Data Custodian runs its own authorization server. ApplicationInformation carries\n      authorizationServerUri, authorizationServerAuthorizationEndpoint,\n      authorizationServerTokenEndpoint and authorizationServerRegistrationEndpoint;\n      GrantType and TokenEndPointMethod select the flow and client authentication method.\n  schema_elements:\n  - authorizationServerUri\n  - authorizationServerAuthorizationEndpoint\n  - authorizationServerTokenEndpoint\n  - authorizationServerRegistrationEndpoint\n  - GrantType\n  - TokenEndPointMethod\n  - scope\n  - OAuthError\n  scopes_note: >-\n    The schema declares a `scope` element and an Authorization resource, but the scope\n    string grammar and its permitted values live in the copyright-protected REQ.21 Model\n    Business Practices narrative, which NAESB paywalls. No scope vocabulary is published\n    openly, so no scopes/ artifact is emitted for this provider rather than guessing\
  \ one.\nunauthenticated_surface:\n- surface: WSDL retrieval\n  url: https://www.naesbwry.oati.com/cgi-bin/webplus.dll?Script=/naesbwry/WREG-Web-Services-Main.wml\n  note: The full 30-operation WSDL is served without any credential.\n- surface: ESPI XML schema download\n  url: https://www.naesb.org/ESPI_Standards.asp\n  note: >-\n    The four ESPI XSDs are downloadable anonymously after a one-click terms-of-use\n    acknowledgement, released under Apache License 2.0 as a documented one-time exception\n    to the NAESB Copyright Policy.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/naesb/refs/heads/main/authentication/naesb-authentication.yml
summary_line: mutualTLS/oauth2 · 2 schemes
tags:
- Energy
- United States
- Standards
- Utilities
- Electricity
- Gas
- Green Button
- Smart Metering
- Energy Markets
- Grid
---
