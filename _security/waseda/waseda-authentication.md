---
api_key_in: []
auth_types:
- saml2
- oauth2
- apiKey
- none
description: How Waseda University's machine-readable surfaces authenticate. Three regimes are in play and they belong to different operators. Waseda's own Shibboleth SAML 2.0 identity provider fronts browser sign-in to campus services and is federation infrastructure rather than an API credential. Waseda Moodle exposes two credentialed programmatic doors on Waseda's own host — LTI 1.3 / LTI Advantage over OAuth 2.0 client credentials, and the Moodle Web Services REST endpoint over a per-user token. Against that, Waseda's read surfaces — the institutional repository's OAI-PMH endpoint and the Waseda IIIF image and manifest servers — are fully anonymous and need no credential at all.
kind: authentication
layout: security
method: probed
name: Waseda Authentication
name_suffix: Authentication
oauth_flows: []
overview: Waseda University secures its APIs with saml2, oauth2, apiKey, and none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Waseda University
provider_slug: waseda
scheme_count: 0
schemes: []
slug: waseda-authentication
source_filename: waseda-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nname: Waseda University — Authentication\ndescription: >-\n  How Waseda University's machine-readable surfaces authenticate. Three regimes are in play and they\n  belong to different operators. Waseda's own Shibboleth SAML 2.0 identity provider fronts browser\n  sign-in to campus services and is federation infrastructure rather than an API credential. Waseda\n  Moodle exposes two credentialed programmatic doors on Waseda's own host — LTI 1.3 / LTI Advantage\n  over OAuth 2.0 client credentials, and the Moodle Web Services REST endpoint over a per-user token.\n  Against that, Waseda's read surfaces — the institutional repository's OAI-PMH endpoint and the\n  Waseda IIIF image and manifest servers — are fully anonymous and need no credential at all.\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  live unauthenticated probes of wsdmoodle.waseda.jp, iaidp.ia.waseda.jp, iiif.archive.waseda.jp and\n  waseda.repo.nii.ac.jp on 2026-09-01. No credentials of any kind were\
  \ used or attempted.\nx-operator: institution\nurl: https://raw.githubusercontent.com/api-evangelist/waseda/main/authentication/waseda-authentication.yml\n\nmechanisms:\n  - id: shibboleth-saml-sso\n    type: saml2\n    label: Waseda Shibboleth SAML 2.0 single sign-on\n    operator: institution\n    entity_id: https://iaidp.ia.waseda.jp/idp/shibboleth\n    scope: waseda.jp\n    endpoints:\n      - binding: HTTP-Redirect\n        purpose: SSO\n        url: https://iaidp.ia.waseda.jp/idp/profile/SAML2/Redirect/SSO\n      - binding: HTTP-POST\n        purpose: SSO\n        url: https://iaidp.ia.waseda.jp/idp/profile/SAML2/POST/SSO\n      - binding: HTTP-POST-SimpleSign\n        purpose: SSO\n        url: https://iaidp.ia.waseda.jp/idp/profile/SAML2/POST-SimpleSign/SSO\n      - binding: SOAP\n        purpose: AttributeQuery\n        url: https://iaidp.ia.waseda.jp:8443/idp/profile/SAML2/SOAP/AttributeQuery\n      - binding: SOAP\n        purpose: ArtifactResolution\n        url: https://iaidp.ia.waseda.jp:8443/idp/profile/SAML2/SOAP/ArtifactResolution\n\
  \    federation:\n      name: GakuNin (学術認証フェデレーション)\n      operator: National Institute of Informatics (NII)\n      metadata: https://metadata.gakunin.nii.ac.jp/gakunin-metadata.xml\n      onward: eduGAIN\n    onboarding: >-\n      Not a public API credential. A relying party obtains access by registering a Service Provider\n      in the GakuNin federation, at which point Waseda's IdP is reachable through the federation\n      metadata. Individuals authenticate with a Waseda ID through MyWaseda.\n    method: probed\n    source: https://iaidp.ia.waseda.jp/idp/shibboleth\n\n  - id: lti13-client-credentials\n    type: oauth2\n    flow: client_credentials\n    label: Waseda Moodle — LTI 1.3 / LTI Advantage service credentials\n    operator: institution\n    token_url: https://wsdmoodle.waseda.jp/mod/lti/token.php\n    authorization_url: https://wsdmoodle.waseda.jp/mod/lti/auth.php\n    jwks_url: https://wsdmoodle.waseda.jp/mod/lti/certs.php\n    service_url: https://wsdmoodle.waseda.jp/mod/lti/services.php\n\
  \    assertion: >-\n      client_assertion_type urn:ietf:params:oauth:client-assertion-type:jwt-bearer — the tool signs a\n      JWT with its own key and the platform verifies it, per the IMS Global Security Framework.\n    scopes_note: >-\n      LTI Advantage scopes (Names and Role Provisioning, Assignment and Grade Services, Deep Linking)\n      are negotiated per registered tool. No scope list is published anonymously, so none is asserted here.\n    observed:\n      - url: https://wsdmoodle.waseda.jp/mod/lti/token.php\n        status: 400\n        body: '{ \"error\" : \"invalid_request\" }'\n      - url: https://wsdmoodle.waseda.jp/mod/lti/certs.php\n        status: 200\n        body_note: JWKS with one RSA/RS256 key, kid ea841dc4e7af7463cc4c\n      - url: https://wsdmoodle.waseda.jp/mod/lti/services.php\n        status: 405\n        body: '{\"status\":405,\"reason\":\"Method Not Allowed\"}'\n    onboarding: >-\n      Tool registration is an administrative act inside Waseda Moodle;\
  \ there is no self-service\n      developer portal and no public registration URL was found.\n    method: probed\n    source: https://wsdmoodle.waseda.jp/mod/lti/certs.php\n\n  - id: moodle-webservice-token\n    type: apiKey\n    in: query\n    parameter_names:\n      - wstoken\n    label: Waseda Moodle Web Services — REST token\n    operator: institution\n    endpoint: https://wsdmoodle.waseda.jp/webservice/rest/server.php\n    observed:\n      - url: https://wsdmoodle.waseda.jp/webservice/rest/server.php\n        status: 200\n        content_type: application/xml; charset=utf-8\n        body: '<EXCEPTION class=\"core\\exception\\moodle_exception\"><ERRORCODE>invalidtoken</ERRORCODE>…'\n        detail: >-\n          The endpoint is deployed and answers an anonymous call with Moodle's structured invalidtoken\n          fault rather than a 404 or a login redirect. Note the HTTP status is 200 — the failure is in\n          the body, so status alone would misread this as an open API.\n  \
  \  onboarding: >-\n      Tokens are issued per user by a Waseda Moodle administrator. No public issuance path exists.\n    method: probed\n    source: https://wsdmoodle.waseda.jp/webservice/rest/server.php\n\n  - id: anonymous-read\n    type: none\n    label: Anonymous read — repository harvesting and IIIF\n    operator: mixed\n    applies_to:\n      - Waseda University Repository OAI-PMH (operator tenant, host waseda.repo.nii.ac.jp)\n      - Waseda IIIF Presentation and Image APIs (operator institution, host iiif.archive.waseda.jp)\n    detail: >-\n      Both answer credential-free GETs with complete payloads. The OAI-PMH endpoint additionally\n      content-negotiates: a browser User-Agent draws 406 from NII's nginx while a plain client gets\n      200, which is a client-shape quirk rather than an access control.\n    method: probed\n    source: https://waseda.repo.nii.ac.jp/oai?verb=Identify\n\n  - id: primo-credentialed\n    type: unknown\n    label: Ex Libris Primo / Alma programmatic\
  \ interfaces (WINE)\n    operator: tenant\n    detail: >-\n      Waseda's WINE discovery service runs on Ex Libris Primo VE. The Primo Search REST and Alma SRU\n      interfaces exist as Ex Libris platform capabilities but are not enabled or documented publicly\n      for Waseda: https://api-ap.hosted.exlibrisgroup.com/view/sru/81SOKEI_INST and the WUNI variant\n      both return 404 SERVICE_NOT_FOUND. Recorded as unknown rather than asserted, and the contract\n      belongs to Ex Libris in any case.\n    observed:\n      - url: https://api-ap.hosted.exlibrisgroup.com/view/sru/81SOKEI_INST?version=1.2&operation=explain\n        status: 404\n      - url: https://waseda.primo.exlibrisgroup.com/discovery/search?vid=81SOKEI_WUNI:WINE\n        status: 200\n        detail: Primo single-page-application shell; a UI, not an API response.\n    method: probed\n    source: https://api-ap.hosted.exlibrisgroup.com/view/sru/81SOKEI_INST?version=1.2&operation=explain\n\nsummary:\n  types:\n    - saml2\n\
  \    - oauth2\n    - apiKey\n    - none\n  public_anonymous_surfaces: 2\n  credentialed_surfaces: 3\n  self_service_key_issuance: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waseda/refs/heads/main/authentication/waseda-authentication.yml
summary_line: saml2/oauth2/apiKey/none · 0 schemes
tags:
- University
- Higher Education
- Education
- Japan
- Asia
- Private Research University
- Research
- Library
- Open Access
- Cultural Heritage
- Digital Archives
- IIIF
- Identity Federation
- Learning Management
- Research Repository
---
