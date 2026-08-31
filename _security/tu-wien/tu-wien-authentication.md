---
api_key_in: []
api_specs:
- filename: tu-wien-fundify-api-openapi.yml
  format: yaml
  label: FUNDify — RIS Synergy Funding API
  slug: fundify-funding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tu-wien/refs/heads/main/openapi/tu-wien-fundify-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Tu Wien Authentication
name_suffix: Authentication
oauth_flows: []
overview: TU Wien declares 7 security scheme(s) across its OpenAPI definitions.
provider_name: TU Wien
provider_slug: tu-wien
scheme_count: 7
schemes:
- detail: 'InvenioRDM. GET /api/records, /api/communities, /api/vocabularies/*, /api/affiliations and /api/funders answer anonymously. /api/names returns 403 anonymously. Write operations (drafts, file upload, curation requests) require a personal access token issued from the user account and sent as `Authorization: Bearer <token>`.'
  evidence:
  - status: 200
    url: https://researchdata.tuwien.ac.at/api/records?size=1
  - status: 403
    url: https://researchdata.tuwien.ac.at/api/names?size=1
  - status: 200
    url: https://researchdata.tuwien.ac.at/tuw/about/api
  scheme: none for read, bearer for write
  surface: tu-wien:researchdata-api
  x-operator: institution
- evidence:
  - status: 200
    url: https://researchdata.tuwien.ac.at/oai2d?verb=Identify
  scheme: none
  surface: tu-wien:researchdata-oai
  x-operator: institution
- evidence:
  - status: 200
    url: https://repositum.tuwien.at/oai/openaire?verb=Identify
  scheme: none
  surface: tu-wien:repositum-oai
  x-operator: institution
- evidence:
  - status: 416
    url: https://repositum.tuwien.at/server/api/core/items?size=1
  - status: 503
    url: https://repositum.tuwien.at/server/api
  scheme: none declared — request refused by a crawler filter before authentication is reached
  surface: tu-wien:repositum-rest
  x-operator: institution
- detail: https://tiss.tuwien.ac.at/api/dokumentation redirects to a TU Wien Login page. The API edge is reachable anonymously and returns a structured XML error document under the namespace https://tiss.tuwien.ac.at/api/schema/error/v10, but resource paths are not publicly enumerable and the documentation that would name them is behind the institutional IdP.
  evidence:
  - detail: page title "TU Wien Login" (unauthenticated); "Cookie fehlt" without a session cookie
    status: 200
    url: https://tiss.tuwien.ac.at/api/dokumentation
  - detail: RESTEasy XML error document — proves a live REST backend behind /api/course/
    status: 404
    url: https://tiss.tuwien.ac.at/api/course/v22/all
  scheme: TU Wien single sign-on
  surface: tu-wien:tiss-api
  x-operator: institution
- detail: Anonymous calls to the funding routes return 401 with an empty body. The source repository configures a Keycloak client against https://id.arisnet.ac.at/realms/fundify; the RIS Synergy network broker realm that TU Wien itself operates publishes a public discovery document.
  evidence:
  - status: 401
    url: https://fundify.arisnet.ac.at/api/ris-synergy/funding/v1/fundings
  - status: 200
    url: https://ris-synergy.csd.tuwien.ac.at/auth/realms/ris-synergy/.well-known/openid-configuration
  scheme: OAuth 2.0 / OpenID Connect bearer token (Keycloak)
  surface: tu-wien:fundify-funding
  x-operator: institution
- detail: entityID https://idp.zid.tuwien.ac.at/saml2, SimpleSAMLphp, registered in the ACOnet / eduID.at federation and interfederated into eduGAIN. This is the credential behind almost every gated TU Wien surface above.
  evidence:
  - status: 200
    url: https://eduid.at/md/aconet-registered.xml
  scheme: SAML 2.0 Web Browser SSO
  surface: tu-wien:saml-idp
  x-operator: institution
slug: tu-wien-authentication
source_filename: tu-wien-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\ngenerated: '2026-08-30'\nmethod: derived\nprobe: true\nprobe_note: >-\n  Written by API Evangelist from live HTTP probes run on 2026-08-30. `derived` is the authorship\n  vocabulary term; every status code recorded below was actually returned to us. TU Wien did not\n  publish this file.\nsource: live probes 2026-08-30 plus the FUNDify contract in openapi/_original/\nsummary: >-\n  TU Wien has no single API gateway and no unified developer credential. Each institution-operated\n  surface carries its own scheme, and three of the five machine surfaces are anonymous-readable.\nschemes:\n  - surface: tu-wien:researchdata-api\n    x-operator: institution\n    scheme: none for read, bearer for write\n    detail: >-\n      InvenioRDM. GET /api/records, /api/communities, /api/vocabularies/*, /api/affiliations and\n      /api/funders answer anonymously. /api/names returns 403 anonymously. Write operations\n      (drafts, file upload, curation requests) require a personal access\
  \ token issued from the user\n      account and sent as `Authorization: Bearer <token>`.\n    evidence:\n      - url: https://researchdata.tuwien.ac.at/api/records?size=1\n        status: 200\n      - url: https://researchdata.tuwien.ac.at/api/names?size=1\n        status: 403\n      - url: https://researchdata.tuwien.ac.at/tuw/about/api\n        status: 200\n  - surface: tu-wien:researchdata-oai\n    x-operator: institution\n    scheme: none\n    evidence:\n      - url: https://researchdata.tuwien.ac.at/oai2d?verb=Identify\n        status: 200\n  - surface: tu-wien:repositum-oai\n    x-operator: institution\n    scheme: none\n    evidence:\n      - url: https://repositum.tuwien.at/oai/openaire?verb=Identify\n        status: 200\n  - surface: tu-wien:repositum-rest\n    x-operator: institution\n    scheme: none declared — request refused by a crawler filter before authentication is reached\n    evidence:\n      - url: https://repositum.tuwien.at/server/api/core/items?size=1\n        status:\
  \ 416\n      - url: https://repositum.tuwien.at/server/api\n        status: 503\n  - surface: tu-wien:tiss-api\n    x-operator: institution\n    scheme: TU Wien single sign-on\n    detail: >-\n      https://tiss.tuwien.ac.at/api/dokumentation redirects to a TU Wien Login page. The API edge is\n      reachable anonymously and returns a structured XML error document under the namespace\n      https://tiss.tuwien.ac.at/api/schema/error/v10, but resource paths are not publicly enumerable\n      and the documentation that would name them is behind the institutional IdP.\n    evidence:\n      - url: https://tiss.tuwien.ac.at/api/dokumentation\n        status: 200\n        detail: 'page title \"TU Wien Login\" (unauthenticated); \"Cookie fehlt\" without a session cookie'\n      - url: https://tiss.tuwien.ac.at/api/course/v22/all\n        status: 404\n        detail: RESTEasy XML error document — proves a live REST backend behind /api/course/\n  - surface: tu-wien:fundify-funding\n    x-operator:\
  \ institution\n    scheme: OAuth 2.0 / OpenID Connect bearer token (Keycloak)\n    detail: >-\n      Anonymous calls to the funding routes return 401 with an empty body. The source repository\n      configures a Keycloak client against https://id.arisnet.ac.at/realms/fundify; the RIS Synergy\n      network broker realm that TU Wien itself operates publishes a public discovery document.\n    evidence:\n      - url: https://fundify.arisnet.ac.at/api/ris-synergy/funding/v1/fundings\n        status: 401\n      - url: https://ris-synergy.csd.tuwien.ac.at/auth/realms/ris-synergy/.well-known/openid-configuration\n        status: 200\n  - surface: tu-wien:saml-idp\n    x-operator: institution\n    scheme: SAML 2.0 Web Browser SSO\n    detail: >-\n      entityID https://idp.zid.tuwien.ac.at/saml2, SimpleSAMLphp, registered in the ACOnet /\n      eduID.at federation and interfederated into eduGAIN. This is the credential behind almost\n      every gated TU Wien surface above.\n    evidence:\n  \
  \    - url: https://eduid.at/md/aconet-registered.xml\n        status: 200\nnot_found:\n  - api key issuance page\n  - developer portal registration\n  - OAuth client self-registration on any TU Wien host\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tu-wien/refs/heads/main/authentication/tu-wien-authentication.yml
summary_line: 7 schemes
tags:
- University
- Higher Education
- Education
- Technical University
- Austria
- Europe
- Research Data
- Research Repository
- Open Access
- OAI-PMH
- Identity Federation
- Research Computing
- InvenioRDM
- DataCite
- ORCID
- SAML
- RIS Synergy
---
