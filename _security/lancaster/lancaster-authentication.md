---
api_key_in: []
api_specs:
- filename: lancaster-oai2-api-openapi.yml
  format: yaml
  label: Lancaster EPrints OAI-PMH 2.0 Interface
  slug: lancaster-oai2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lancaster/refs/heads/main/openapi/lancaster-oai2-api-openapi.yml
- filename: lancaster-identityfederation-api-openapi.yml
  format: yaml
  label: Lancaster Shibboleth Identity Provider (SAML 2.0 metadata)
  slug: identity-federation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lancaster/refs/heads/main/openapi/lancaster-identityfederation-api-openapi.yml
auth_types: []
description: Lancaster University publishes no API key programme, no developer registration and no OAuth authorisation server of its own. Its one open machine-readable API is unauthenticated; its identity surface is the authentication system itself; everything else on a lancaster.ac.uk or lancs.ac.uk hostname that a client might want is behind institutional single sign-on.
kind: authentication
layout: security
method: probed
name: Lancaster Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lancaster University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Lancaster University
provider_slug: lancaster
scheme_count: 0
schemes: []
slug: lancaster-authentication
source_filename: lancaster-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: >-\n  Authentication posture observed by probing Lancaster University-operated hosts on 2026-08-30.\n  Each statement below names the surface it applies to; no posture is generalised across\n  surfaces, because Lancaster's differ sharply.\nprovider: Lancaster University\nproviderId: lancaster\ndescription: >-\n  Lancaster University publishes no API key programme, no developer registration and no OAuth\n  authorisation server of its own. Its one open machine-readable API is unauthenticated; its\n  identity surface is the authentication system itself; everything else on a lancaster.ac.uk or\n  lancs.ac.uk hostname that a client might want is behind institutional single sign-on.\nsurfaces:\n- api: lancaster:lancaster-oai2-api\n  name: Lancaster EPrints OAI-PMH 2.0 interface\n  x-operator: institution\n  scheme: none\n  registration: none\n  evidence:\n    url: https://eprints.lancs.ac.uk/cgi/oai2?verb=Identify\n    status: 200\n\
  \    detail: >-\n      Anonymous GET returns a full Identify response with no credential, no key parameter and no\n      WWW-Authenticate challenge. Selective harvesting, ListSets and ListRecords are equally open.\n  rights_note: >-\n    Open does not mean licensed. The Identify response's eprints description block returns\n    \"No metadata policy defined. This server has not yet been fully configured... if in doubt\n    assume that NO rights at all are granted to this data\", and the same wording for the data\n    and submission policies. Harvesting is technically unrestricted and legally undeclared;\n    https://eprints.lancs.ac.uk/policies.html is the URL the repository itself points at.\n- api: lancaster:identity-federation\n  name: Lancaster Shibboleth Identity Provider (SAML 2.0)\n  x-operator: institution\n  scheme: saml2\n  registration: federation\n  evidence:\n    url: https://idp.lancs.ac.uk/idp/shibboleth\n    status: 200\n    detail: >-\n      The metadata document is served\
  \ anonymously - that is the point of it. Using the IdP,\n      as opposed to reading its metadata, requires the relying party to be a registered UK\n      Access Federation or eduGAIN service provider; attribute release is governed by the\n      federation, not by a self-service developer signup.\n  endpoints:\n    sso_post: https://idp.lancs.ac.uk/idp/profile/SAML2/POST/SSO\n    sso_redirect: https://idp.lancs.ac.uk/idp/profile/SAML2/Redirect/SSO\n    attribute_query: https://idp.lancs.ac.uk:8443/idp/profile/SAML2/SOAP/AttributeQuery\n    artifact_resolution: https://idp.lancs.ac.uk:8443/idp/profile/SAML2/SOAP/ArtifactResolution\n- api: lancaster:student-portal\n  name: iLancaster / Lancaster portal\n  x-operator: institution\n  scheme: sso\n  registration: institutional_account\n  evidence:\n    url: https://portal.lancaster.ac.uk/\n    status: 200\n    detail: >-\n      Redirects to https://weblogin.lancs.ac.uk/login/?cosign-https-cosign2.lancs.ac.uk with a\n      JWT handoff (jwt/auth_any.php?ID=PortalLive).\
  \ Lancaster runs CoSign for local web SSO\n      alongside Shibboleth for federated access. No anonymous data is reachable behind it, so no\n      contract is described here.\n- api: lancaster:pure-research-directory\n  name: Elsevier Pure research directory\n  x-operator: tenant\n  scheme: vendor_controlled\n  detail: >-\n    Pure's /ws/api web service responds on the tenant host but rejects unversioned requests -\n    HTTP 500 with body {\"timestamp\":...,\"status\":999,\"error\":\"None\"}. Keys for it are issued by\n    Elsevier through the institution's Pure administrators, not by a Lancaster developer programme.\n- api: lancaster:library-discovery\n  name: Ex Libris Alma / Primo VE\n  x-operator: tenant\n  scheme: vendor_controlled\n  detail: >-\n    Alma API keys are issued through the Ex Libris Developer Network against the institution's\n    Alma instance. Lancaster operates the tenancy; Ex Libris operates the key programme.\nabsent:\n- api_keys\n- oauth2\n- openid_connect_discovery\n\
  - developer_registration\n- mtls\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lancaster/refs/heads/main/authentication/lancaster-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- United Kingdom
- N8 Research Partnership
- Research Data
- Institutional Repository
- Identity Federation
- Library
- Open Source
---
