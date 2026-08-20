---
api_key_in: []
api_specs:
- filename: princeton-allsearch-api-openapi.yml
  format: yaml
  label: Princeton University Library Allsearch API
  slug: allsearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-allsearch-api-openapi.yml
- filename: princeton-art-museum-api-openapi.yml
  format: yaml
  label: Princeton University Art Museum API
  slug: art-museum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-art-museum-api-openapi.yml
auth_types:
- none
- oauth2
- saml
description: ''
kind: authentication
layout: security
method: probed
name: Princeton Authentication
name_suffix: Authentication
oauth_flows:
- client_credentials
overview: Princeton University secures its APIs with none, oauth2, and saml across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the client_credentials flow(s).
provider_name: Princeton University
provider_slug: princeton
scheme_count: 4
schemes:
- applies_to:
  - Princeton University Library Allsearch API (allsearch-api.princeton.edu)
  - Princeton University Art Museum API (data.artmuseum.princeton.edu)
  - Blacklight discovery JSON (catalog / figgy / dpul / findingaids / maps / datacommons)
  description: No credential of any kind. The Allsearch OpenAPI declares no securitySchemes and no security block, and anonymous GETs returned 200 on every probed path. The Art Museum documentation states plainly that "no authentication is currently required to access the API, however this may change in future versions" — an honest forward-looking caveat, recorded as such.
  name: NoAuthentication
  type: none
  verified:
  - status: 200
    url: https://allsearch-api.princeton.edu/search/catalog?query=climate
  - status: 200
    url: https://data.artmuseum.princeton.edu/objects/9449/tombstone
  x-operator: institution
- applies_to:
  - Princeton OIT API Gateway (api.princeton.edu)
  description: The OIT enterprise gateway runs WSO2 API Manager (probes return an am:fault envelope in the http://wso2.org/apimanager namespace). Calls without a bearer token return 401 with an empty body. Subscription requires a Princeton NetID or a departmental service account, so the surface is gated to the campus community rather than to the public. The API Store portal that used to front it, api-store.princeton.edu, no longer resolves (NXDOMAIN as of 2026-08-19).
  flow: client_credentials
  name: PrincetonAPIGatewayOAuth2
  type: oauth2
  verified:
  - status: 401
    url: https://api.princeton.edu/active-directory/1.0.6/users
  - note: WSO2 am:fault "No matching resource found" — the gateway is live, this path is not published.
    status: 404
    url: https://api.princeton.edu/registrar/course-offerings
  x-operator: institution
- applies_to:
  - Princeton campus web single sign-on (idp.princeton.edu)
  description: Institutional web SSO is Shibboleth/SAML 2.0. The IdP publishes signed metadata at https://idp.princeton.edu/idp/shibboleth (SAML 2.0 + SAML 1.1 protocol support, shibmd:Scope, signing and encryption keys). This is the only identity contract Princeton publishes machine-readably, and it is entirely institution-operated.
  name: ShibbolethSAML
  type: saml
  verified:
  - status: 200
    url: https://idp.princeton.edu/idp/shibboleth
  x-operator: institution
- applies_to:
  - Princeton University Library staff applications (bibdata.princeton.edu)
  description: PUL applications expose a staff login at /users/auth/cas backed by Princeton CAS. Public read operations on those hosts do not require it; write and administrative operations do.
  name: CASLogin
  type: cas
  verified:
  - status: 200
    url: https://bibdata.princeton.edu/
  x-operator: institution
slug: princeton-authentication
source_filename: princeton-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: live Princeton-operated hosts, probed 2026-08-19\nx-operator: institution\nnote: >-\n  Princeton's programmable surface splits cleanly into two authentication postures: the Library's\n  public discovery APIs, which require nothing at all, and the OIT enterprise gateway, which\n  requires a NetID or service-account OAuth2 token and is unreachable to the public. Recorded from\n  probes and from the published OpenAPI, not from a marketing page.\nsummary:\n  types: [none, oauth2, saml]\n  api_key_in: []\n  oauth2_flows: [client_credentials]\nschemes:\n- name: NoAuthentication\n  type: none\n  applies_to:\n  - Princeton University Library Allsearch API (allsearch-api.princeton.edu)\n  - Princeton University Art Museum API (data.artmuseum.princeton.edu)\n  - Blacklight discovery JSON (catalog / figgy / dpul / findingaids / maps / datacommons)\n  description: >-\n    No credential of any kind. The Allsearch OpenAPI declares no securitySchemes\
  \ and no security\n    block, and anonymous GETs returned 200 on every probed path. The Art Museum documentation\n    states plainly that \"no authentication is currently required to access the API, however this\n    may change in future versions\" — an honest forward-looking caveat, recorded as such.\n  x-operator: institution\n  verified:\n  - url: https://allsearch-api.princeton.edu/search/catalog?query=climate\n    status: 200\n  - url: https://data.artmuseum.princeton.edu/objects/9449/tombstone\n    status: 200\n- name: PrincetonAPIGatewayOAuth2\n  type: oauth2\n  flow: client_credentials\n  applies_to:\n  - Princeton OIT API Gateway (api.princeton.edu)\n  description: >-\n    The OIT enterprise gateway runs WSO2 API Manager (probes return an am:fault envelope in the\n    http://wso2.org/apimanager namespace). Calls without a bearer token return 401 with an empty\n    body. Subscription requires a Princeton NetID or a departmental service account, so the\n    surface is gated to the\
  \ campus community rather than to the public. The API Store portal that\n    used to front it, api-store.princeton.edu, no longer resolves (NXDOMAIN as of 2026-08-19).\n  x-operator: institution\n  verified:\n  - url: https://api.princeton.edu/active-directory/1.0.6/users\n    status: 401\n  - url: https://api.princeton.edu/registrar/course-offerings\n    status: 404\n    note: WSO2 am:fault \"No matching resource found\" — the gateway is live, this path is not published.\n- name: ShibbolethSAML\n  type: saml\n  applies_to:\n  - Princeton campus web single sign-on (idp.princeton.edu)\n  description: >-\n    Institutional web SSO is Shibboleth/SAML 2.0. The IdP publishes signed metadata at\n    https://idp.princeton.edu/idp/shibboleth (SAML 2.0 + SAML 1.1 protocol support,\n    shibmd:Scope, signing and encryption keys). This is the only identity contract Princeton\n    publishes machine-readably, and it is entirely institution-operated.\n  x-operator: institution\n  verified:\n  - url:\
  \ https://idp.princeton.edu/idp/shibboleth\n    status: 200\n- name: CASLogin\n  type: cas\n  applies_to:\n  - Princeton University Library staff applications (bibdata.princeton.edu)\n  description: >-\n    PUL applications expose a staff login at /users/auth/cas backed by Princeton CAS. Public read\n    operations on those hosts do not require it; write and administrative operations do.\n  x-operator: institution\n  verified:\n  - url: https://bibdata.princeton.edu/\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/authentication/princeton-authentication.yml
summary_line: none/oauth2/saml · 4 schemes
tags:
- University
- Higher Education
- Education
- Ivy League
- United States
- New Jersey
- Research Library
- Research Data
- Open Data
- Digital Collections
- Identity Federation
- Museum
---
