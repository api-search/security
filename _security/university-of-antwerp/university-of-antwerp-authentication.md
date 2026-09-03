---
api_key_in: []
api_specs:
- filename: university-of-antwerp-irua-oai-pmh-openapi.yml
  format: yaml
  label: IRUA OAI-PMH Metadata Interface
  slug: irua-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-antwerp/refs/heads/main/openapi/university-of-antwerp-irua-oai-pmh-openapi.yml
auth_types: []
description: 'How access is established across the University of Antwerp''s surfaces. There is no API key programme, no OAuth authorization server the institution operates for third parties, and no developer registration of any kind. Access is binary: metadata harvesting is fully anonymous, and everything else is behind institutional SAML single sign-on.'
kind: authentication
layout: security
method: probed
name: University Of Antwerp Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Antwerp declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: University of Antwerp
provider_slug: university-of-antwerp
scheme_count: 5
schemes:
- detail: No authentication. Every OAI-PMH verb answered HTTP 200 to an anonymous client with no header, key or referrer. No rate limiting was observed, including on a ListRecords call that returned 2,826,135 bytes; that is an absence of evidence, not a documented guarantee.
  scheme: none
  surface: IRUA OAI-PMH metadata harvesting
  url: https://repository.uantwerpen.be/oai/abua/
  x-operator: institution
- detail: Shibboleth Identity Provider, SAML 2.0 with HTTP-Redirect, HTTP-POST and HTTP-POST-SimpleSign SSO bindings plus a SAML 1.1/2.0 attribute authority over SOAP. shibmd:Scope ua.ac.be. Registered in the Belnet R&E Federation and interfederated into eduGAIN, so an eligible relying party obtains access through federation membership rather than through anything the university issues directly. This is the institution's real authorization contract and it is machine-readable. See identity-federation/university-of-antwerp-identity-federation.yml.
  scheme: saml2
  surface: Institutional single sign-on
  url: https://idpx.ua.ac.be/idp/shibboleth
  x-operator: institution
- detail: Form login against the Brocade/Wander application, session propagated as a numeric `session` query parameter across framesets. Public OPAC views are reachable anonymously; staff functions are not. No documented programmatic authentication.
  scheme: proprietary-session
  surface: Wander / Brocade library platform
  url: https://go.wander.be/
  x-operator: institution
- detail: 'Anthology''s Blackboard Learn REST API is reachable on the university''s hostname: /learn/api/public/v1/system/version returns HTTP 200 with a version document (learn 4000.21.0, build rel.28+435d029), while /learn/api/public/v1/courses returns HTTP 401 {"status":401,"message":"API request is not authenticated."}. Blackboard''s REST API uses OAuth 2.0 with developer keys issued per-institution. The contract, the OAuth server and the engineering are Anthology''s; the tenancy is the university''s. Recorded, not credited.'
  scheme: oauth2
  surface: Blackboard Learn (Anthology)
  url: https://blackboard.uantwerpen.be/learn/api/public/v1/
  x-operator: tenant
- detail: Redirects to a Shibboleth discovery service whose institution list includes "Universiteit Antwerpen" against entityID https://idpx.ua.ac.be/idp/shibboleth — the university's own IdP authenticating into a consortium service that Ghent University operates (157.193.43.57, RUGNET1).
  scheme: saml2
  surface: Flemish Supercomputer Centre account portal
  url: https://account.vscentrum.be/
  x-operator: tenant
slug: university-of-antwerp-authentication
source_filename: university-of-antwerp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Evangelist Authentication\nspecificationVersion: '0.1'\nprovider: University of Antwerp\nproviderId: university-of-antwerp\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  Anonymous probes of https://repository.uantwerpen.be/oai/abua/ (all verbs, HTTP 200 with no\n  credential); https://idpx.ua.ac.be/idp/shibboleth (HTTP 200, SAML 2.0 metadata);\n  https://blackboard.uantwerpen.be/learn/api/public/v1/system/version (HTTP 200) and\n  /learn/api/public/v1/courses (HTTP 401); https://go.wander.be/ (login form); and\n  https://account.vscentrum.be/ (Shibboleth WAYF redirect). All 2026-09-01.\ndescription: >-\n  How access is established across the University of Antwerp's surfaces. There is no API key\n  programme, no OAuth authorization server the institution operates for third parties, and no\n  developer registration of any kind. Access is binary: metadata harvesting is fully anonymous,\n  and everything else is behind institutional SAML single sign-on.\n\
  schemes:\n- surface: IRUA OAI-PMH metadata harvesting\n  url: https://repository.uantwerpen.be/oai/abua/\n  x-operator: institution\n  scheme: none\n  detail: >-\n    No authentication. Every OAI-PMH verb answered HTTP 200 to an anonymous client with no\n    header, key or referrer. No rate limiting was observed, including on a ListRecords call\n    that returned 2,826,135 bytes; that is an absence of evidence, not a documented guarantee.\n- surface: Institutional single sign-on\n  url: https://idpx.ua.ac.be/idp/shibboleth\n  x-operator: institution\n  scheme: saml2\n  detail: >-\n    Shibboleth Identity Provider, SAML 2.0 with HTTP-Redirect, HTTP-POST and\n    HTTP-POST-SimpleSign SSO bindings plus a SAML 1.1/2.0 attribute authority over SOAP.\n    shibmd:Scope ua.ac.be. Registered in the Belnet R&E Federation and interfederated into\n    eduGAIN, so an eligible relying party obtains access through federation membership rather\n    than through anything the university issues directly.\
  \ This is the institution's real\n    authorization contract and it is machine-readable.\n    See identity-federation/university-of-antwerp-identity-federation.yml.\n- surface: Wander / Brocade library platform\n  url: https://go.wander.be/\n  x-operator: institution\n  scheme: proprietary-session\n  detail: >-\n    Form login against the Brocade/Wander application, session propagated as a numeric\n    `session` query parameter across framesets. Public OPAC views are reachable anonymously;\n    staff functions are not. No documented programmatic authentication.\n- surface: Blackboard Learn (Anthology)\n  url: https://blackboard.uantwerpen.be/learn/api/public/v1/\n  x-operator: tenant\n  scheme: oauth2\n  detail: >-\n    Anthology's Blackboard Learn REST API is reachable on the university's hostname:\n    /learn/api/public/v1/system/version returns HTTP 200 with a version document\n    (learn 4000.21.0, build rel.28+435d029), while /learn/api/public/v1/courses returns\n    HTTP 401 {\"\
  status\":401,\"message\":\"API request is not authenticated.\"}. Blackboard's REST\n    API uses OAuth 2.0 with developer keys issued per-institution. The contract, the OAuth\n    server and the engineering are Anthology's; the tenancy is the university's. Recorded, not\n    credited.\n- surface: Flemish Supercomputer Centre account portal\n  url: https://account.vscentrum.be/\n  x-operator: tenant\n  scheme: saml2\n  detail: >-\n    Redirects to a Shibboleth discovery service whose institution list includes \"Universiteit\n    Antwerpen\" against entityID https://idpx.ua.ac.be/idp/shibboleth — the university's own\n    IdP authenticating into a consortium service that Ghent University operates\n    (157.193.43.57, RUGNET1).\nabsent:\n  api_keys: No API key issuance, developer portal or registration flow found on any host.\n  oauth_authorization_server: >-\n    None operated by the institution. The only OAuth in evidence belongs to Anthology\n    (Blackboard) and to ORCID, both third parties.\n\
  \  well_known: >-\n    https://www.uantwerpen.be/.well-known/security.txt returns 404, and no\n    /.well-known/oauth-protected-resource or openid-configuration was found on any\n    institution host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-antwerp/refs/heads/main/authentication/university-of-antwerp-authentication.yml
summary_line: 5 schemes
tags:
- Education
- Higher Education
- University
- Belgium
- Europe
- Flanders
- Institutional Repository
- OAI-PMH
- Identity Federation
- Library
- Research Repository
- Research Computing
- Learning Management
---
