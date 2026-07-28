---
api_key_in: []
api_specs:
- filename: southern-california-edison-drpep-arcgis-openapi.yml
  format: yaml
  label: SCE DRPEP ArcGIS REST Services
  slug: sce-drpep-arcgis-rest-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/southern-california-edison/refs/heads/main/openapi/southern-california-edison-drpep-arcgis-openapi.yml
auth_types:
- none
- oauth2
- token
description: ''
kind: authentication
layout: security
method: searched
name: Southern California Edison Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Southern California Edison secures its APIs with none, oauth2, and token across 0 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Southern California Edison
provider_slug: southern-california-edison
scheme_count: 0
schemes: []
slug: southern-california-edison-authentication
source_filename: southern-california-edison-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  https://www.sce.com/partners/3rd-party-energy-providers/access-energy-usage-data +\n  https://drpep.sce.com/arcgis_server/rest/info?f=json + https://sce.okta.com/.well-known/openid-configuration\ndocs: https://www.sce.com/partners/partnerships/thirdpartylandingpage\nsummary:\n  types: [none, oauth2, token]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  note: >-\n    Two disjoint surfaces. The one API a developer can call today (DRPEP ArcGIS REST) has NO authentication\n    at all. The one API SCE is compelled by tariff to operate (Green Button Connect My Data) is stated to use\n    OAuth 2.0 but publishes no authorization endpoint, token endpoint, scope list, client-registration flow or\n    redirect-URI policy anywhere public. Nothing in the OAuth column below was observed on the wire; it is\n    SCE's own written claim plus the tariff text, recorded as a claim.\nsurfaces:\n- name: SCE DRPEP ArcGIS REST Services\n\
  \  api: openapi/southern-california-edison-drpep-arcgis-openapi.yml\n  scheme: none\n  status: verified\n  evidence: >-\n    https://drpep.sce.com/arcgis_server/rest/services/Hosted?f=json and every hosted FeatureServer /query\n    under it return HTTP 200 JSON with no token, no key, no cookie and no registration (verified 2026-07-27).\n  notes:\n  - >-\n    /arcgis_server/rest/info reports authInfo.isTokenBasedSecurity = true with a token service at\n    https://drpep.sce.com/arcgis_portal/sharing/rest/generateToken. That describes the ArcGIS Enterprise\n    deployment, not the public sharing of the Hosted folder - the Hosted services are shared publicly and\n    answer anonymously.\n  - >-\n    The sibling folder /arcgis_server/rest/services/Utilities is NOT public: it returns HTTP 200 with\n    {\"error\":{\"code\":499,\"message\":\"Token Required\"}}. Anyone needing it must obtain an ArcGIS token from\n    generateToken, which requires an SCE-issued portal account.\n  - No API key,\
  \ no rate-limit header, no per-caller identity of any kind is issued for the public layers.\n- name: SCE Green Button Connect My Data (Customer Data Access)\n  api: null\n  scheme: oauth2\n  status: claimed-undisclosed\n  claimed_flow: authorizationCode\n  evidence: >-\n    SCE's third-party page states a third party must have \"technical system capabilities to complete customer\n    authorization using OAuth 2.0 and process files that are transferred using bulk API\", and that the program\n    \"leverages technology consistent with the standard adopted by the North American Energy Standards Board\n    (NAESB) to support the Green Button Initiative\". CPUC tariff Rule 26 (Advice 3087-E, effective 2014-08-29,\n    implementing D.14-05-016) requires machine-to-machine verification and ties technical eligibility to the\n    NAESB ESPI Standard.\n  undisclosed:\n  - authorization endpoint\n  - token endpoint\n  - base URI / resource endpoint\n  - ApplicationInformation document (NAESB ESPI\
  \ client registration)\n  - scope syntax (ESPI FB=/ scope strings)\n  - token lifetime / refresh policy\n  - sandbox or test client\n  gate:\n    type: application-approval\n    steps:\n    - Create a Third Party User ID (an email not already an SCE.com user ID) at https://www.sce.com/user-registration?userType=4\n    - Supply the organization's Taxpayer Identification Number (TIN)\n    - Accept the Third Party Registration Terms & Conditions for use of customer data\n    - Pass an SCE-run machine-to-machine connectivity test\n    contact: mailto:GreenButton@sce.com\n  probe_result: >-\n    api.sce.com is live (Imperva -> IBM DataPower / API Connect) but every ESPI-shaped path probed\n    (/espi/1_1/resource/ApplicationInformation, /DataCustodian/espi/1_1/..., /greenbutton/..., /oauth/token)\n    returned HTTP 500 with the gateway fault \"Dynamic backend host not specified\". Real gateway, no anonymous route.\n- name: SCE Okta identity org\n  api: null\n  scheme: openIdConnect\n  status:\
  \ verified\n  discovery: https://sce.okta.com/.well-known/openid-configuration\n  artifact: well-known/southern-california-edison-okta-openid-configuration.json\n  evidence: >-\n    Anonymous HTTP 200. issuer https://sce.okta.com; authorization_endpoint /oauth2/v1/authorize;\n    token_endpoint /oauth2/v1/token; jwks_uri /oauth2/v1/keys; grant types authorization_code, implicit,\n    refresh_token, password, device_code (plus client_credentials on the RFC 8414 document); PKCE S256.\n  caveat: >-\n    This is the login estate for sce.com / My Account / the Energy Data Request Program shell. It is NOT\n    evidence of a Green Button OAuth surface and must not be presented as one.\nscopes:\n  published: false\n  note: >-\n    No energy-data scope list exists publicly. The scopes advertised by sce.okta.com are Okta's own platform\n    scopes (openid/email/profile plus okta.* management scopes) and describe Okta, not SCE customer data - so\n    no scopes/ artifact is emitted for this provider\
  \ rather than fabricate one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/southern-california-edison/refs/heads/main/authentication/southern-california-edison-authentication.yml
summary_line: none/oauth2/token · 0 schemes
tags:
- Energy
- United States
- Utilities
- Electricity
- Smart Metering
- Green Button
- Grid
- Demand Response
- Solar
- DER
- EV Charging
- California
---
