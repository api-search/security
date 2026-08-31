---
api_key_in: []
api_specs:
- filename: tokyo-institute-of-technology-t2r2-oaipmh-openapi.yml
  format: yaml
  label: T2R2 Research Repository OAI-PMH
  slug: t2r2-oaipmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tokyo-institute-of-technology/refs/heads/main/openapi/tokyo-institute-of-technology-t2r2-oaipmh-openapi.yml
auth_types:
- saml2
description: ''
kind: authentication
layout: security
method: derived
name: Tokyo Institute Of Technology Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tokyo Institute of Technology secures its APIs with saml2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tokyo Institute of Technology
provider_slug: tokyo-institute-of-technology
scheme_count: 2
schemes:
- audience: Members of the institution and of GakuNin-federated services. Not issuable to third-party developers.
  display_name: Institute of Science Tokyo (Science & Engineering Field)
  endpoints:
  - binding: urn:mace:shibboleth:1.0:profiles:AuthnRequest
    location: https://idp-gakunin.nap.gsic.titech.ac.jp/idp/profile/Shibboleth/SSO
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
    location: https://idp-gakunin.nap.gsic.titech.ac.jp/idp/profile/SAML2/POST/SSO
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
    location: https://idp-gakunin.nap.gsic.titech.ac.jp/idp/profile/SAML2/Redirect/SSO
  - binding: urn:oasis:names:tc:SAML:1.0:bindings:SOAP-binding
    location: https://idp-gakunin.nap.gsic.titech.ac.jp:8443/idp/profile/SAML1/SOAP/AttributeQuery
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:SOAP
    location: https://idp-gakunin.nap.gsic.titech.ac.jp:8443/idp/profile/SAML2/SOAP/AttributeQuery
  entity_id: https://idp-gakunin.nap.gsic.titech.ac.jp/idp/shibboleth
  federation: GakuNin (Academic Access Management Federation in Japan), operated by NII
  metadata_source: https://metadata.gakunin.nii.ac.jp/gakunin-metadata.xml
  name: GakuNin Shibboleth IdP (Science & Engineering field)
  observed: GET https://idp-gakunin.nap.gsic.titech.ac.jp/idp/shibboleth redirects (HTTP 200) to the institution's own login portal at portal.nap.gsic.titech.ac.jp with resource id idp-gakunin-2015 and an authentication-factor list including CERTIFICATE, GRID, TOKENRO and OTP. Probed 2026-08-30.
  operator: institution
  organization: Institute of Science Tokyo / 東京科学大学
  organization_url: https://portal.titech.ac.jp/
  type: saml2
- endpoints:
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
    location: https://isct.ex-tic.com/auth/gakunin/saml2/assertions
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
    location: https://isct.ex-tic.com/auth/gakunin/saml2/assertions
  entity_id: https://isct.ex-tic.com/auth/gakunin/saml2/assertions
  federation: GakuNin
  metadata_source: https://metadata.gakunin.nii.ac.jp/gakunin-metadata.xml
  name: EX-TIC GakuNin entity for Institute of Science Tokyo
  observed: A bare GET returns HTTP 400 — correct for a SAML assertion endpoint that expects a POST, and not evidence of a dead host. Probed 2026-08-30.
  operator: tenant
  operator_note: The host is an institution-specific subdomain on ex-tic.com, a commercial platform. The institution's identity is real and federated here; the engineering is the vendor's. Recorded as a tenant relationship, which is a genuine institutional fact, rather than credited to the institution or deleted.
  organization: Institute of Science Tokyo / 東京科学大学
  organization_url: https://www.tmd.ac.jp
  type: saml2
slug: tokyo-institute-of-technology-authentication
source_filename: tokyo-institute-of-technology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: derived\nevidence_method: probed\nevidence_note: >-\n  Derived by API Evangelist from the live GakuNin federation metadata aggregate plus direct\n  probes of the advertised endpoints on 2026-08-30. The institution publishes no authentication\n  document of its own.\nsource: https://metadata.gakunin.nii.ac.jp/gakunin-metadata.xml\ndocs: https://www.gakunin.jp/en\nnote: >-\n  This institution publishes no OAuth 2.0 or OpenID Connect developer API. Its authentication\n  posture is entirely federated SAML: a Shibboleth Identity Provider registered in GakuNin,\n  Japan's national academic access management federation. That is a real, machine-readable,\n  institution-operated interface — it is simply not a developer API, and must not be counted as\n  one. The one public harvesting endpoint the institution runs (T2R2 OAI-PMH) requires no\n  authentication at all.\nsummary:\n  types:\n  - saml2\n  api_key_in: []\n  oauth2_flows: []\n  public_unauthenticated_surfaces:\n\
  \  - https://t2r2.star.titech.ac.jp/oaipmh/OAIHandler\n  note: >-\n    No signup, no API key, no bearer token and no rate-limit headers were observed on the\n    OAI-PMH endpoint. No /.well-known/openid-configuration and no /.well-known/oauth-authorization-server\n    was found on any institution host.\nschemes:\n- name: GakuNin Shibboleth IdP (Science & Engineering field)\n  type: saml2\n  operator: institution\n  entity_id: https://idp-gakunin.nap.gsic.titech.ac.jp/idp/shibboleth\n  organization: Institute of Science Tokyo / 東京科学大学\n  display_name: Institute of Science Tokyo (Science & Engineering Field)\n  organization_url: https://portal.titech.ac.jp/\n  federation: GakuNin (Academic Access Management Federation in Japan), operated by NII\n  metadata_source: https://metadata.gakunin.nii.ac.jp/gakunin-metadata.xml\n  endpoints:\n  - binding: urn:mace:shibboleth:1.0:profiles:AuthnRequest\n    location: https://idp-gakunin.nap.gsic.titech.ac.jp/idp/profile/Shibboleth/SSO\n  - binding:\
  \ urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n    location: https://idp-gakunin.nap.gsic.titech.ac.jp/idp/profile/SAML2/POST/SSO\n  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n    location: https://idp-gakunin.nap.gsic.titech.ac.jp/idp/profile/SAML2/Redirect/SSO\n  - binding: urn:oasis:names:tc:SAML:1.0:bindings:SOAP-binding\n    location: https://idp-gakunin.nap.gsic.titech.ac.jp:8443/idp/profile/SAML1/SOAP/AttributeQuery\n  - binding: urn:oasis:names:tc:SAML:2.0:bindings:SOAP\n    location: https://idp-gakunin.nap.gsic.titech.ac.jp:8443/idp/profile/SAML2/SOAP/AttributeQuery\n  observed: >-\n    GET https://idp-gakunin.nap.gsic.titech.ac.jp/idp/shibboleth redirects (HTTP 200) to the\n    institution's own login portal at portal.nap.gsic.titech.ac.jp with resource id\n    idp-gakunin-2015 and an authentication-factor list including CERTIFICATE, GRID, TOKENRO and\n    OTP. Probed 2026-08-30.\n  audience: Members of the institution and of GakuNin-federated services.\
  \ Not issuable to third-party developers.\n- name: EX-TIC GakuNin entity for Institute of Science Tokyo\n  type: saml2\n  operator: tenant\n  entity_id: https://isct.ex-tic.com/auth/gakunin/saml2/assertions\n  organization: Institute of Science Tokyo / 東京科学大学\n  organization_url: https://www.tmd.ac.jp\n  federation: GakuNin\n  metadata_source: https://metadata.gakunin.nii.ac.jp/gakunin-metadata.xml\n  endpoints:\n  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n    location: https://isct.ex-tic.com/auth/gakunin/saml2/assertions\n  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n    location: https://isct.ex-tic.com/auth/gakunin/saml2/assertions\n  observed: >-\n    A bare GET returns HTTP 400 — correct for a SAML assertion endpoint that expects a POST, and\n    not evidence of a dead host. Probed 2026-08-30.\n  operator_note: >-\n    The host is an institution-specific subdomain on ex-tic.com, a commercial platform. The\n    institution's identity is real and\
  \ federated here; the engineering is the vendor's. Recorded\n    as a tenant relationship, which is a genuine institutional fact, rather than credited to the\n    institution or deleted.\nabsent:\n- id: oauth2\n  evidence: No authorization or token endpoint published on any institution host.\n- id: oidc\n  evidence: /.well-known/openid-configuration not served on isct.ac.jp or titech.ac.jp hosts probed.\n- id: api-key\n  evidence: No key issuance surface, no developer portal, no signup flow found.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tokyo-institute-of-technology/refs/heads/main/authentication/tokyo-institute-of-technology-authentication.yml
summary_line: saml2 · 2 schemes
tags:
- Education
- Higher Education
- University
- Institute of Technology
- Japan
- Research
- Research Data
- Open Access
- Institutional Repository
- OAI-PMH
- Identity Federation
- Shibboleth
- SAML
- Research Computing
- Course Catalog
- Library
---
