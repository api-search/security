---
api_key_in: []
api_specs:
- filename: university-of-manchester-iiif-presentation-api-openapi.yml
  format: yaml
  label: Manchester Digital Collections — IIIF Presentation API
  slug: iiif-presentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-manchester/refs/heads/main/openapi/university-of-manchester-iiif-presentation-api-openapi.yml
- filename: university-of-manchester-iiif-image-api-openapi.yml
  format: yaml
  label: Manchester Digital Collections — IIIF Image API
  slug: iiif-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-manchester/refs/heads/main/openapi/university-of-manchester-iiif-image-api-openapi.yml
auth_types:
- saml2
- none
description: ''
kind: authentication
layout: security
method: probed
name: University Of Manchester Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Manchester secures its APIs with saml2 and none across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Manchester
provider_slug: university-of-manchester
scheme_count: 2
schemes:
- description: Shibboleth Identity Provider for staff, students and federated e-resource access. Registered in the Jisc UK Access Management Federation (and through it eduGAIN) under entityID https://shib.manchester.ac.uk/shibboleth, asserting the scope manchester.ac.uk. This is institutional single sign-on infrastructure, not a developer API — no application can obtain a token from it without being registered as a service provider in the federation.
  display_name: University of Manchester
  endpoints:
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
    location: https://shib.manchester.ac.uk/shibboleth-idp/profile/SAML2/Redirect/SSO
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
    location: https://shib.manchester.ac.uk/shibboleth-idp/profile/SAML2/POST/SSO
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign
    location: https://shib.manchester.ac.uk/shibboleth-idp/profile/SAML2/POST-SimpleSign/SSO
  - binding: urn:mace:shibboleth:1.0:profiles:AuthnRequest
    location: https://shib.manchester.ac.uk/shibboleth-idp/profile/Shibboleth/SSO
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:SOAP
    location: https://shib.manchester.ac.uk:8443/shibboleth-idp/profile/SAML2/SOAP/ArtifactResolution
  entity_id: https://shib.manchester.ac.uk/shibboleth
  metadata:
    bytes: 9647
    document: authentication/university-of-manchester-saml-idp-metadata.xml
    method: searched
    retrieved: '2026-08-19'
    retrieved_from: http://mdq.ukfederation.org.uk/entities/https%3A%2F%2Fshib.manchester.ac.uk%2Fshibboleth
    signed: true
    status: 200
  name: shibboleth-saml2
  organization_name: The University of Manchester
  protocols:
  - urn:mace:shibboleth:1.0
  - urn:oasis:names:tc:SAML:1.1:protocol
  - urn:oasis:names:tc:SAML:2.0:protocol
  scope: manchester.ac.uk
  sources:
  - http://mdq.ukfederation.org.uk/entities/https%3A%2F%2Fshib.manchester.ac.uk%2Fshibboleth
  type: saml2
  x-operator: institution
- description: The Manchester Digital Collections IIIF Presentation and Image APIs require no authentication. Manifests, collections, info.json documents and image derivatives were all retrieved anonymously on 2026-08-19 and returned 200. There is no key, no token and no registration step.
  name: iiif-anonymous
  sources:
  - https://www.digitalcollections.manchester.ac.uk/iiif/MS-LATIN-00006
  - https://image.digitalcollections.manchester.ac.uk/iiif/MS-LATIN-00006-000-00001.jp2/info.json
  type: none
  x-operator: institution
slug: university-of-manchester-authentication
source_filename: university-of-manchester-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\ngenerated: '2026-08-19'\nmethod: probed\nsource: >-\n  Live probes on 2026-08-19 of the University of Manchester's own authentication surfaces, plus\n  the institution's signed SAML entity descriptor retrieved from the UK Access Management\n  Federation MDQ service.\nx-operator: institution\n\nsummary:\n  note: >-\n    The University of Manchester operates no public OAuth authorization server and issues no\n    self-service API credentials. Its institution-operated authentication is federated SAML for\n    people, and its institution-operated machine surfaces are open and unauthenticated.\n  types:\n  - saml2\n  - none\n  public_oauth: false\n  self_serve_api_keys: false\n\nschemes:\n- name: shibboleth-saml2\n  type: saml2\n  x-operator: institution\n  description: >-\n    Shibboleth Identity Provider for staff, students and federated e-resource access. Registered in\n    the Jisc UK Access Management Federation (and through it eduGAIN) under entityID\n    https://shib.manchester.ac.uk/shibboleth,\
  \ asserting the scope manchester.ac.uk. This is\n    institutional single sign-on infrastructure, not a developer API — no application can obtain a\n    token from it without being registered as a service provider in the federation.\n  entity_id: https://shib.manchester.ac.uk/shibboleth\n  scope: manchester.ac.uk\n  organization_name: The University of Manchester\n  display_name: University of Manchester\n  protocols:\n  - urn:mace:shibboleth:1.0\n  - urn:oasis:names:tc:SAML:1.1:protocol\n  - urn:oasis:names:tc:SAML:2.0:protocol\n  endpoints:\n  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n    location: https://shib.manchester.ac.uk/shibboleth-idp/profile/SAML2/Redirect/SSO\n  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n    location: https://shib.manchester.ac.uk/shibboleth-idp/profile/SAML2/POST/SSO\n  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign\n    location: https://shib.manchester.ac.uk/shibboleth-idp/profile/SAML2/POST-SimpleSign/SSO\n\
  \  - binding: urn:mace:shibboleth:1.0:profiles:AuthnRequest\n    location: https://shib.manchester.ac.uk/shibboleth-idp/profile/Shibboleth/SSO\n  - binding: urn:oasis:names:tc:SAML:2.0:bindings:SOAP\n    location: https://shib.manchester.ac.uk:8443/shibboleth-idp/profile/SAML2/SOAP/ArtifactResolution\n  metadata:\n    document: authentication/university-of-manchester-saml-idp-metadata.xml\n    retrieved_from: http://mdq.ukfederation.org.uk/entities/https%3A%2F%2Fshib.manchester.ac.uk%2Fshibboleth\n    retrieved: '2026-08-19'\n    status: 200\n    bytes: 9647\n    signed: true\n    method: searched\n  sources:\n  - http://mdq.ukfederation.org.uk/entities/https%3A%2F%2Fshib.manchester.ac.uk%2Fshibboleth\n\n- name: iiif-anonymous\n  type: none\n  x-operator: institution\n  description: >-\n    The Manchester Digital Collections IIIF Presentation and Image APIs require no authentication.\n    Manifests, collections, info.json documents and image derivatives were all retrieved anonymously\n\
  \    on 2026-08-19 and returned 200. There is no key, no token and no registration step.\n  sources:\n  - https://www.digitalcollections.manchester.ac.uk/iiif/MS-LATIN-00006\n  - https://image.digitalcollections.manchester.ac.uk/iiif/MS-LATIN-00006-000-00001.jp2/info.json\n\nnot_operated_by_institution:\n- name: pure-api-key\n  type: apiKey\n  x-operator: tenant\n  description: >-\n    The Pure CRIS REST API at pure.manchester.ac.uk/ws/api is gated by an `api-key` request header.\n    The scheme is Elsevier's, defined in Elsevier's Pure product specification, and the same header\n    gates every Pure customer's instance. Manchester administers the keys for its own tenancy; it\n    did not design the mechanism. Recorded here for completeness and deliberately excluded from\n    `schemes` so it is not credited to the institution.\n  host: pure.manchester.ac.uk\n  cname: uom-aws.elsevierpure.com\n- name: figshare-oauth\n  type: oauth2\n  x-operator: vendor\n  description: >-\n    Figshare's\
  \ OAuth 2.0 authorization, operated by Figshare for all customers at\n    api.figshare.com. Manchester is a tenant at figshare.manchester.ac.uk; the authorization server\n    is not Manchester's.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-manchester/refs/heads/main/authentication/university-of-manchester-authentication.yml
summary_line: saml2/none · 2 schemes
tags:
- University
- Higher Education
- Education
- Research
- United Kingdom
- Russell Group
- Library
- Digital Collections
- IIIF
- Identity Federation
- Research Data
- Research Computing
---
