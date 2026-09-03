---
api_key_in:
- header
api_specs:
- filename: tietoevry-openbanking-xs2a-swagger.json
  format: json
  label: Tietoevry Open Banking XS2A APIs
  slug: tietoevry-openbanking-xs2a
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tietoevry/refs/heads/main/openapi/tietoevry-openbanking-xs2a-swagger.json
- filename: tietoevry-financial-api-aggregation-swagger.json
  format: json
  label: Tietoevry Financial API Aggregation
  slug: tietoevry-financial-api-aggregation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tietoevry/refs/heads/main/openapi/tietoevry-financial-api-aggregation-swagger.json
- filename: tietoevry-sepa-direct-debit-api-gateway.yaml
  format: yaml
  label: Tietoevry SEPA Direct Debits
  slug: tietoevry-sepa-direct-debits
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tietoevry/refs/heads/main/openapi/tietoevry-sepa-direct-debit-api-gateway.yaml
auth_types:
- apiKey
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Tietoevry Authentication
name_suffix: Authentication
oauth_flows: []
overview: TietoEVRY secures its APIs with apiKey, openIdConnect, and mutualTLS across 7 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TietoEVRY
provider_slug: tietoevry
scheme_count: 7
schemes:
- description: The API key of the application registered in My Apps. The provider manual states it "must be added to every call you make on our APIs" and it is copied from the app detail screen in the portal. Present as a required header parameter on 171 published operations.
  in: header
  name: APIKeyHeader
  obtained_at: https://openbanking.api.tietoevry.com/workplace/applications/sandbox
  parameter: X-API-Key
  scope: all XS2A, premium and VAM operations
  sources:
  - openapi/tietoevry-tieto-xs2a-vam-accounts.yaml
  - openapi/tietoevry-tieto-xs2a-vam-users.yaml
  - https://openbanking.api.tietoevry.com/documentation/how-to-instruction.yaml
  type: apiKey
- description: OAuth 2.0 bearer access token used for the OAuth2 SCA (redirect) and embedded SCA approaches described in the provider's oauth2-how-to and embedded-SCA introductions. Declared as an Authorization header parameter on 62 operations rather than as a securityScheme; the provider publishes no authorization-server metadata document and no scope reference, so the token endpoint and scope names are not machine-readable from the public surface.
  name: Authorization
  scheme: bearer
  sources:
  - openapi/tietoevry-oauth2-how-to.yaml
  - openapi/tietoevry-tieto-oauth2-embedded-intro.yaml
  type: http
- description: Declared on the SEPA Direct Debits gateway. The URL is an unreplaced placeholder, so the discovery document cannot be fetched; treat the real issuer as undocumented.
  name: bearerToken
  openIdConnectUrl: http://example/openid-connect
  sources:
  - openapi/tietoevry-sepa-direct-debit-api-gateway.yaml
  type: openIdConnect
- applies_to: live
  description: PSD2 production access requires eIDAS qualified certificates (QWAC for transport, QSealC for sealing), registered against the application in the portal. The provider manual states "QWAC and QSeal certificates are not required in the Sandbox mode", which is the reverse statement of the live requirement. Consistent with this, https://openbanking.api.tieto.com (the host named in the published specs as the live XS2A base) resolves to 20.86.199.14 but terminates TLS with a self-signed chain to an ordinary client, i.e. the live gateway is not reachable without the client certificate.
  name: eIDAS QWAC / QSealC
  sources:
  - https://openbanking.api.tietoevry.com/documentation/how-to-instruction.yaml
  - probe of https://openbanking.api.tieto.com/ on 2026-09-02
  type: mutualTLS
- description: Application ID to be used for authentication against Generic SSO.
  in: header
  name: APPIDHeader
  parameter: X-APP-ID
  scope: VAM
  sources:
  - openapi/tietoevry-tieto-xs2a-vam-accounts.yaml
  - openapi/tietoevry-tieto-xs2a-vam-users.yaml
  type: apiKey
- description: Token to be used for authentication against Generic SSO.
  in: header
  name: TokenHeader
  parameter: X-Token
  scope: VAM
  sources:
  - openapi/tietoevry-tieto-xs2a-vam-accounts.yaml
  - openapi/tietoevry-tieto-xs2a-vam-users.yaml
  type: apiKey
- description: Token type to be used for authentication against Generic SSO. This provides support for different types of token by different issuing systems.
  in: header
  name: TokenTypeHeader
  parameter: X-Token-Type
  scope: VAM
  sources:
  - openapi/tietoevry-tieto-xs2a-vam-accounts.yaml
  - openapi/tietoevry-tieto-xs2a-vam-users.yaml
  type: apiKey
slug: tietoevry-authentication
source_filename: tietoevry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://openbanking.api.tietoevry.com/documentation/how-to-instruction.yaml (provider \"Getting\n  started!\" manual, fetched 2026-09-02, HTTP 200), plus the securityDefinitions declared in\n  openapi/tietoevry-tieto-xs2a-vam-accounts.yaml, openapi/tietoevry-tieto-xs2a-vam-users.yaml and\n  openapi/tietoevry-sepa-direct-debit-api-gateway.yaml\ndocs: https://openbanking.api.tietoevry.com/getting-started\nnote: 'Spec-derived security is thin because the Berlin Group XS2A specs Tietoevry publishes declare their\n  credential headers as ordinary header parameters rather than securityDefinitions: X-API-Key appears as a\n  required header parameter on 171 of the 211 published operations but is a declared securityScheme only in\n  the two VAM specs. The provider manual states the real profile, so this file is upgraded from derived to\n  searched. The openIdConnectUrl in the SEPA Direct Debits gateway spec is the literal placeholder\n\
  \  http://example/openid-connect and does not resolve to a Tietoevry issuer.'\nsummary:\n  types:\n  - apiKey\n  - openIdConnect\n  - mutualTLS\n  api_key_in:\n  - header\n  primary: 'API key in the X-API-Key header, issued per registered application in the developer portal'\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'The API key of the application registered in My Apps. The provider manual states it \"must be\n    added to every call you make on our APIs\" and it is copied from the app detail screen in the portal.\n    Present as a required header parameter on 171 published operations.'\n  scope: all XS2A, premium and VAM operations\n  obtained_at: https://openbanking.api.tietoevry.com/workplace/applications/sandbox\n  sources:\n  - openapi/tietoevry-tieto-xs2a-vam-accounts.yaml\n  - openapi/tietoevry-tieto-xs2a-vam-users.yaml\n  - https://openbanking.api.tietoevry.com/documentation/how-to-instruction.yaml\n- name: Authorization\n\
  \  type: http\n  scheme: bearer\n  description: 'OAuth 2.0 bearer access token used for the OAuth2 SCA (redirect) and embedded SCA approaches\n    described in the provider''s oauth2-how-to and embedded-SCA introductions. Declared as an Authorization\n    header parameter on 62 operations rather than as a securityScheme; the provider publishes no\n    authorization-server metadata document and no scope reference, so the token endpoint and scope names are\n    not machine-readable from the public surface.'\n  sources:\n  - openapi/tietoevry-oauth2-how-to.yaml\n  - openapi/tietoevry-tieto-oauth2-embedded-intro.yaml\n- name: bearerToken\n  type: openIdConnect\n  openIdConnectUrl: http://example/openid-connect\n  description: 'Declared on the SEPA Direct Debits gateway. The URL is an unreplaced placeholder, so the\n    discovery document cannot be fetched; treat the real issuer as undocumented.'\n  sources:\n  - openapi/tietoevry-sepa-direct-debit-api-gateway.yaml\n- name: eIDAS QWAC / QSealC\n\
  \  type: mutualTLS\n  description: 'PSD2 production access requires eIDAS qualified certificates (QWAC for transport, QSealC for\n    sealing), registered against the application in the portal. The provider manual states \"QWAC and QSeal\n    certificates are not required in the Sandbox mode\", which is the reverse statement of the live\n    requirement. Consistent with this, https://openbanking.api.tieto.com (the host named in the published\n    specs as the live XS2A base) resolves to 20.86.199.14 but terminates TLS with a self-signed chain to an\n    ordinary client, i.e. the live gateway is not reachable without the client certificate.'\n  applies_to: live\n  sources:\n  - https://openbanking.api.tietoevry.com/documentation/how-to-instruction.yaml\n  - probe of https://openbanking.api.tieto.com/ on 2026-09-02\n- name: APPIDHeader\n  type: apiKey\n  in: header\n  parameter: X-APP-ID\n  description: Application ID to be used for authentication against Generic SSO.\n  scope: VAM\n  sources:\n\
  \  - openapi/tietoevry-tieto-xs2a-vam-accounts.yaml\n  - openapi/tietoevry-tieto-xs2a-vam-users.yaml\n- name: TokenHeader\n  type: apiKey\n  in: header\n  parameter: X-Token\n  description: Token to be used for authentication against Generic SSO.\n  scope: VAM\n  sources:\n  - openapi/tietoevry-tieto-xs2a-vam-accounts.yaml\n  - openapi/tietoevry-tieto-xs2a-vam-users.yaml\n- name: TokenTypeHeader\n  type: apiKey\n  in: header\n  parameter: X-Token-Type\n  description: Token type to be used for authentication against Generic SSO. This provides support for\n    different types of token by different issuing systems.\n  scope: VAM\n  sources:\n  - openapi/tietoevry-tieto-xs2a-vam-accounts.yaml\n  - openapi/tietoevry-tieto-xs2a-vam-users.yaml\nconsent_model:\n  note: 'Beyond credentials, every account-data and funds-confirmation call carries a Consent-ID header\n    naming a PSU consent that the customer authorised through an SCA redirect. Consent is the real\n    authorisation object in this\
  \ API, not a scope.'\n  header: Consent-ID\n  statuses:\n  - received\n  - valid\n  - rejected\n  - expired\n  - revokedByPsu\n  - terminatedByTpp\n  - blocked\n  - deleted\n  max_validity: 'Recurring AIS consent validity is 90 days, extended to 180 days under the EBA SCA exemption\n    in Commission Delegated Regulation (EU) 2022/2360 RTS Article 10a; the provider states the 180-day\n    interface is available in the Sandbox environment.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tietoevry/refs/heads/main/authentication/tietoevry-authentication.yml
summary_line: apiKey/openIdConnect/mutualTLS · 7 schemes
tags:
- Company
- Banking
- Open Banking
- PSD2
- XS2A
- Berlin Group
- Payments
- SEPA
- Account Information
- Financial Services
- Aggregation
- Credit
- Fintech
- Nordic
- Finland
---
