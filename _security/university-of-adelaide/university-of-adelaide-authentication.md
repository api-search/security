---
api_key_in: []
auth_types:
- saml2
- cas
- oidc
description: The University of Adelaide operates its own authentication estate and does not publish a public API authorization server. Every credentialed surface below terminates at an institution-controlled identity provider; none issues tokens to an unaffiliated developer. The public, keyless surface of this institution — the DSpace REST API and its OAI-PMH endpoint — requires no authentication at all for read access.
kind: authentication
layout: security
method: probed
name: University Of Adelaide Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Adelaide secures its APIs with saml2, cas, and oidc across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Adelaide
provider_slug: university-of-adelaide
scheme_count: 4
schemes:
- bindings:
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign
  entity_id: urn:mace:federation.org.au:testfed:au-idp.adelaide.edu.au
  evidence: examples/university-of-adelaide-saml-idp-metadata.xml
  federation: Australian Access Federation (AAF)
  federation_metadata: https://md.aaf.edu.au/aaf-metadata.xml
  metadata_url: https://au-idp.adelaide.edu.au/idp/shibboleth
  name: Shibboleth SAML 2.0 Identity Provider
  scope: adelaide.edu.au
  sso_endpoints:
  - https://au-idp.adelaide.edu.au/idp/profile/SAML2/Redirect/SSO
  - https://au-idp.adelaide.edu.au/idp/profile/SAML2/POST/SSO
  status: 200
  type: saml2
  x-operator: institution
- login_url: https://login.adelaide.edu.au/cas/login
  name: Central Authentication Service (CAS)
  notes: Institution-hosted CAS single sign-on. Web SSO for staff and student applications; not an API authorization server and issues no developer-facing tokens.
  status: 200
  type: cas
  x-operator: institution
- entry_point: https://id.adelaide.edu.au/
  name: Okta workforce SSO (SAML service provider)
  notes: access.adelaide.edu.au (the student system) 302s to an Okta-hosted SAML endpoint on the institution-specific subdomain id.adelaide.edu.au. Okta is the vendor; the tenant is the institution's.
  status: 200
  type: saml2
  x-operator: tenant
- authorization_endpoint: https://myuni.adelaide.edu.au/login/oauth2/auth
  discovery_url: https://myuni.adelaide.edu.au/.well-known/openid-configuration
  issuer: https://myuni.adelaide.edu.au
  jwks_uri: https://myuni.adelaide.edu.au/login/oauth2/jwks
  lti_jwks_uri: https://myuni.adelaide.edu.au/api/lti/security/jwks
  name: Canvas / MyUni OpenID Connect + LTI 1.3
  notes: Instructure Canvas LMS on the institution's own hostname. The OIDC discovery document and LTI JWKS are publicly readable; the REST API at /api/v1 returns 401 {"status":"unauthenticated"} and issues developer keys only through institutional admin approval.
  status: 200
  token_endpoint: https://myuni.adelaide.edu.au/login/oauth2/token
  type: oidc
  x-operator: tenant
slug: university-of-adelaide-authentication
source_filename: university-of-adelaide-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: >-\n  live HTTP probes of adelaide.edu.au authentication hosts and the Australian Access Federation\n  metadata aggregate, 2026-08-30. Replaces a 2026-07-11 artifact that was derived from Figshare's\n  generic OAuth 2.0 contract and described Figshare's authorization server, not the institution's.\ndescription: >-\n  The University of Adelaide operates its own authentication estate and does not publish a public\n  API authorization server. Every credentialed surface below terminates at an institution-controlled\n  identity provider; none issues tokens to an unaffiliated developer. The public, keyless surface of\n  this institution — the DSpace REST API and its OAI-PMH endpoint — requires no authentication at\n  all for read access.\nsummary:\n  types:\n  - saml2\n  - cas\n  - oidc\n  public_read_without_credentials: true\n  developer_self_service_tokens: false\nschemes:\n- name: Shibboleth SAML 2.0 Identity Provider\n  type:\
  \ saml2\n  x-operator: institution\n  entity_id: urn:mace:federation.org.au:testfed:au-idp.adelaide.edu.au\n  metadata_url: https://au-idp.adelaide.edu.au/idp/shibboleth\n  scope: adelaide.edu.au\n  federation: Australian Access Federation (AAF)\n  federation_metadata: https://md.aaf.edu.au/aaf-metadata.xml\n  bindings:\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign\n  sso_endpoints:\n  - https://au-idp.adelaide.edu.au/idp/profile/SAML2/Redirect/SSO\n  - https://au-idp.adelaide.edu.au/idp/profile/SAML2/POST/SSO\n  status: 200\n  evidence: examples/university-of-adelaide-saml-idp-metadata.xml\n- name: Central Authentication Service (CAS)\n  type: cas\n  x-operator: institution\n  login_url: https://login.adelaide.edu.au/cas/login\n  status: 200\n  notes: >-\n    Institution-hosted CAS single sign-on. Web SSO for staff and student applications; not an API\n    authorization\
  \ server and issues no developer-facing tokens.\n- name: Okta workforce SSO (SAML service provider)\n  type: saml2\n  x-operator: tenant\n  entry_point: https://id.adelaide.edu.au/\n  status: 200\n  notes: >-\n    access.adelaide.edu.au (the student system) 302s to an Okta-hosted SAML endpoint on the\n    institution-specific subdomain id.adelaide.edu.au. Okta is the vendor; the tenant is the\n    institution's.\n- name: Canvas / MyUni OpenID Connect + LTI 1.3\n  type: oidc\n  x-operator: tenant\n  issuer: https://myuni.adelaide.edu.au\n  discovery_url: https://myuni.adelaide.edu.au/.well-known/openid-configuration\n  authorization_endpoint: https://myuni.adelaide.edu.au/login/oauth2/auth\n  token_endpoint: https://myuni.adelaide.edu.au/login/oauth2/token\n  jwks_uri: https://myuni.adelaide.edu.au/login/oauth2/jwks\n  lti_jwks_uri: https://myuni.adelaide.edu.au/api/lti/security/jwks\n  status: 200\n  notes: >-\n    Instructure Canvas LMS on the institution's own hostname. The OIDC discovery\
  \ document and LTI\n    JWKS are publicly readable; the REST API at /api/v1 returns\n    401 {\"status\":\"unauthenticated\"} and issues developer keys only through institutional admin\n    approval.\nunauthenticated_surfaces:\n- url: https://digital.library.adelaide.edu.au/server/api\n  status: 200\n  notes: DSpace REST read access requires no credentials; /server/api/authn advertises the login methods for write operations.\n- url: https://digital.library.adelaide.edu.au/server/oai/request?verb=Identify\n  status: 200\n  notes: OAI-PMH harvesting is open.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/authentication/university-of-adelaide-authentication.yml
summary_line: saml2/cas/oidc · 4 schemes
tags:
- University
- Higher Education
- Education
- Australia
- Group of Eight
- Research Repository
- Research Data
- Library
- OAI-PMH
- DSpace
- Identity Federation
- Shibboleth
- Metadata
- Course Catalog
---
