---
api_key_in: []
auth_types:
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Energyhub Authentication
name_suffix: Authentication
oauth_flows: []
overview: EnergyHub secures its APIs with mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: EnergyHub
provider_slug: energyhub
scheme_count: 2
schemes:
- api: energyhub:mercury-edge-connect-api
  consistent_with: OpenADR 2.0b VEN/VTN security, which is built on TLS with mutual certificate authentication. EnergyHub states the MEC API is "based on the Open ADR standard" but does not name a profile or version, so this is a consistency observation, not a provider claim.
  credential_issuance: EnergyHub issues client certificates to DER partners under a commercial partner agreement; there is no public CSR, enrollment, or certificate-request process.
  evidence: 'Every anonymous request to https://mec.energyhub.com - on /, /openapi.json, /swagger.json,

    /docs, /api-docs, /health, /v1, /api, /oadr, and all six /.well-known/* paths - returns

    HTTP/1.1 400 Bad Request with the nginx body "400 No required SSL certificate was sent".

    That is nginx `ssl_verify_client on`: the server demands an X.509 client certificate during

    the TLS handshake and rejects the request before any routing or application logic runs.

    Server certificate: CN=mec.energyhub.com, issuer "C=US, O=DigiCert Inc, CN=RapidSSL TLS RSA

    CA G1", valid 2026-03-17 to 2026-10-01. Re-probed 2026-07-27 22:23 UTC, identical response.

    '
  host: https://mec.energyhub.com
  name: mutualTLS
  status: confirmed-by-probe
  type: mutualTLS
- evidence: 'Every technical article path on the ClickHelp knowledge base returns HTTP 200 with a

    login interstitial titled "Login" carrying a "Log in with Okta SSO" button and an

    authenticator-code (MFA) field - including /articles/mec/mec-overview and

    /articles/technical-guides/technical-guides-overview. No OIDC discovery document is

    exposed (/.well-known/openid-configuration returns the same login HTML, a soft 404),

    so the issuer, endpoints, and scopes cannot be read anonymously.

    '
  host: https://help.energyhub.com
  name: okta-sso
  note: This gates the documentation, not the runtime API. The ChargingRewards end-user guide section of the same portal is public and requires no login.
  scope: documentation portal only, not the API
  status: confirmed-by-probe
  type: openIdConnect
slug: energyhub-authentication
source_filename: energyhub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: live anonymous probes of mec.energyhub.com and help.energyhub.com, plus the\n  EnergyHub Mercury Edge Connect announcement\nprovider_documented: false\nprovider_documentation_note: |\n  EnergyHub publishes no authentication documentation. There is no developer portal, no auth\n  guide, no key-issuance page, no OAuth endpoint, and no self-serve credential of any kind on\n  any public EnergyHub property. Everything below was established by direct anonymous probing\n  of live hosts on 2026-07-27, not from provider documentation. The MEC integration guides\n  that would describe authentication live at help.energyhub.com/articles/mec/* behind an\n  Okta SSO wall.\nsummary:\n  types: [mutualTLS]\n  api_key_in: []\n  oauth2_flows: []\n  public_credentials: false\n  self_serve_signup: false\nschemes:\n- name: mutualTLS\n  type: mutualTLS\n  api: energyhub:mercury-edge-connect-api\n  host: https://mec.energyhub.com\n  status: confirmed-by-probe\n\
  \  evidence: |\n    Every anonymous request to https://mec.energyhub.com - on /, /openapi.json, /swagger.json,\n    /docs, /api-docs, /health, /v1, /api, /oadr, and all six /.well-known/* paths - returns\n    HTTP/1.1 400 Bad Request with the nginx body \"400 No required SSL certificate was sent\".\n    That is nginx `ssl_verify_client on`: the server demands an X.509 client certificate during\n    the TLS handshake and rejects the request before any routing or application logic runs.\n    Server certificate: CN=mec.energyhub.com, issuer \"C=US, O=DigiCert Inc, CN=RapidSSL TLS RSA\n    CA G1\", valid 2026-03-17 to 2026-10-01. Re-probed 2026-07-27 22:23 UTC, identical response.\n  credential_issuance: EnergyHub issues client certificates to DER partners under a commercial\n    partner agreement; there is no public CSR, enrollment, or certificate-request process.\n  consistent_with: OpenADR 2.0b VEN/VTN security, which is built on TLS with mutual\n    certificate authentication. EnergyHub\
  \ states the MEC API is \"based on the Open ADR\n    standard\" but does not name a profile or version, so this is a consistency observation,\n    not a provider claim.\n- name: okta-sso\n  type: openIdConnect\n  scope: documentation portal only, not the API\n  host: https://help.energyhub.com\n  status: confirmed-by-probe\n  evidence: |\n    Every technical article path on the ClickHelp knowledge base returns HTTP 200 with a\n    login interstitial titled \"Login\" carrying a \"Log in with Okta SSO\" button and an\n    authenticator-code (MFA) field - including /articles/mec/mec-overview and\n    /articles/technical-guides/technical-guides-overview. No OIDC discovery document is\n    exposed (/.well-known/openid-configuration returns the same login HTML, a soft 404),\n    so the issuer, endpoints, and scopes cannot be read anonymously.\n  note: This gates the documentation, not the runtime API. The ChargingRewards end-user\n    guide section of the same portal is public and requires no\
  \ login.\nnot_found:\n- {scheme: apiKey, note: no API key issuance, header, or query parameter is documented anywhere}\n- {scheme: http-basic, note: not offered}\n- {scheme: http-bearer, note: not offered}\n- {scheme: oauth2, note: no authorization server, token endpoint, or scope reference published}\n- {scheme: openIdConnect, note: 'no discovery document on any API host; Okta covers docs SSO only'}\naccess_gate:\n  gate: partner-only\n  path: https://www.energyhub.com/der-partner-ecosystem/become-a-partner\n  note: A \"Connect with us\" lead form. There is no published technical criteria, no sandbox,\n    and no self-serve credential.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/energyhub/refs/heads/main/authentication/energyhub-authentication.yml
summary_line: mutualTLS · 2 schemes
tags:
- Energy
- United States
- Utilities
- Electricity
- Grid
- DERMS
- Distributed Energy Resources
- Demand Response
- Virtual Power Plant
- OpenADR
- EV Charging
- Solar
- Energy Storage
- Smart Thermostats
---
