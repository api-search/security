---
api_key_in: []
auth_types:
- none
- oauth2
- openIdConnect
- saml2
description: ''
kind: authentication
layout: security
method: probed
name: University Of Liverpool Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Liverpool secures its APIs with none, oauth2, openIdConnect, and saml2 across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Liverpool
provider_slug: university-of-liverpool
scheme_count: 5
schemes:
- description: Unauthenticated public read. Applies to both OAI-PMH providers and to the EPrints REST dataset listings on livrepository.liverpool.ac.uk.
  name: anonymous
  operator: institution
  probes:
  - note: 200 with curl's default User-Agent or an OAI harvester UA; 403 (Apache "Forbidden", 295 bytes) with a desktop-browser User-Agent. The host is live — a browser-UA probe alone misgrades it.
    status: 200
    url: https://livrepository.liverpool.ac.uk/cgi/oai2?verb=Identify
  - status: 200
    url: https://datacat.liverpool.ac.uk/cgi/oai2?verb=Identify
  - note: 7,456,493 bytes of eprint-id listing returned with no credentials.
    status: 200
    url: https://livrepository.liverpool.ac.uk/rest/eprint/
  type: none
- authorization_endpoint: https://fs.liverpool.ac.uk/adfs/oauth2/authorize/
  description: Institution-operated Active Directory Federation Services authorization server. Discovery document is public and keyless; the endpoints behind it are not.
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://fs.liverpool.ac.uk/adfs
  jwks_uri: https://fs.liverpool.ac.uk/adfs/discovery/keys
  name: adfs-oauth2-oidc
  openIdConnectUrl: https://fs.liverpool.ac.uk/adfs/.well-known/openid-configuration
  operator: institution
  probes:
  - status: 200
    url: https://fs.liverpool.ac.uk/adfs/.well-known/openid-configuration
  - note: One RSA signing key, 2,524 bytes.
    status: 200
    url: https://fs.liverpool.ac.uk/adfs/discovery/keys
  token_endpoint: https://fs.liverpool.ac.uk/adfs/oauth2/token/
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  - windows_client_authentication
  type: openIdConnect
  userinfo_endpoint: https://fs.liverpool.ac.uk/adfs/userinfo
- description: The institution's Microsoft Entra ID tenant, discoverable by its own domain. Microsoft hosts it; the tenant is Liverpool's.
  issuer: https://login.microsoftonline.com/53255131-b129-4010-86e1-474bfd7e8076/v2.0
  name: entra-id-tenant
  openIdConnectUrl: https://login.microsoftonline.com/liverpool.ac.uk/v2.0/.well-known/openid-configuration
  operator: federation
  probes:
  - status: 200
    url: https://login.microsoftonline.com/liverpool.ac.uk/v2.0/.well-known/openid-configuration
  tenant_region_scope: EU
  type: openIdConnect
- bindings:
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign
  description: Institution-operated Shibboleth SAML 2.0 identity provider, published in the UK Access Management Federation and self-published on its own host.
  entity_id: urn:mace:eduserv.org.uk:athens:provider:liv.ac.uk
  metadata_urls:
  - http://mdq.ukfederation.org.uk/entities/urn%3Amace%3Aeduserv.org.uk%3Aathens%3Aprovider%3Aliv.ac.uk
  - https://shibboleth3.liv.ac.uk/idp/shibboleth
  name: shibboleth-saml2
  operator: federation
  probes:
  - status: 200
    url: http://mdq.ukfederation.org.uk/entities/urn%3Amace%3Aeduserv.org.uk%3Aathens%3Aprovider%3Aliv.ac.uk
  - status: 200
    url: https://shibboleth3.liv.ac.uk/idp/shibboleth
  - note: Live IdP rejecting a parameterless AuthnRequest.
    status: 400
    url: https://shibboleth3.liv.ac.uk/idp/profile/SAML2/Redirect/SSO
  scope: liv.ac.uk
  type: saml2
- description: AD FS SAML 2.0 / WS-Federation metadata for the institution's primary SP-initiated login.
  entity_id: http://fs.liverpool.ac.uk/adfs/services/trust
  metadata_urls:
  - https://fs.liverpool.ac.uk/FederationMetadata/2007-06/FederationMetadata.xml
  name: adfs-saml2
  operator: institution
  probes:
  - note: 83,212 bytes, application/samlmetadata+xml.
    status: 200
    url: https://fs.liverpool.ac.uk/FederationMetadata/2007-06/FederationMetadata.xml
  sso_location: https://fs.liverpool.ac.uk/adfs/ls/
  type: saml2
slug: university-of-liverpool-authentication
source_filename: university-of-liverpool-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live probes of University of Liverpool hosts on 2026-09-01. No OpenAPI exists for any of these\n  surfaces, so every scheme below was read from an actual response — a discovery document, a SAML\n  metadata document, or the status code and body returned to an unauthenticated request.\nnote: >-\n  The institution's public machine surfaces split cleanly in two. Everything scholarly — the two\n  EPrints OAI-PMH providers and the EPrints REST read interface — is open and anonymous, with no key,\n  no token and no registration. Everything else is behind the institution's own identity plane\n  (AD FS, Shibboleth, Entra ID) or a vendor tenant's, and there is no self-service key issuance or\n  developer registration anywhere on the public surface.\nsummary:\n  types:\n  - none\n  - oauth2\n  - openIdConnect\n  - saml2\n  self_service_key_issuance: false\n  developer_registration: false\nschemes:\n- name: anonymous\n  type: none\n\
  \  description: >-\n    Unauthenticated public read. Applies to both OAI-PMH providers and to the EPrints REST dataset\n    listings on livrepository.liverpool.ac.uk.\n  operator: institution\n  probes:\n  - url: https://livrepository.liverpool.ac.uk/cgi/oai2?verb=Identify\n    status: 200\n    note: >-\n      200 with curl's default User-Agent or an OAI harvester UA; 403 (Apache \"Forbidden\", 295 bytes)\n      with a desktop-browser User-Agent. The host is live — a browser-UA probe alone misgrades it.\n  - url: https://datacat.liverpool.ac.uk/cgi/oai2?verb=Identify\n    status: 200\n  - url: https://livrepository.liverpool.ac.uk/rest/eprint/\n    status: 200\n    note: 7,456,493 bytes of eprint-id listing returned with no credentials.\n- name: adfs-oauth2-oidc\n  type: openIdConnect\n  description: >-\n    Institution-operated Active Directory Federation Services authorization server. Discovery\n    document is public and keyless; the endpoints behind it are not.\n  operator: institution\n\
  \  openIdConnectUrl: https://fs.liverpool.ac.uk/adfs/.well-known/openid-configuration\n  issuer: https://fs.liverpool.ac.uk/adfs\n  authorization_endpoint: https://fs.liverpool.ac.uk/adfs/oauth2/authorize/\n  token_endpoint: https://fs.liverpool.ac.uk/adfs/oauth2/token/\n  userinfo_endpoint: https://fs.liverpool.ac.uk/adfs/userinfo\n  jwks_uri: https://fs.liverpool.ac.uk/adfs/discovery/keys\n  id_token_signing_alg_values_supported: [ RS256 ]\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  - windows_client_authentication\n  probes:\n  - url: https://fs.liverpool.ac.uk/adfs/.well-known/openid-configuration\n    status: 200\n  - url: https://fs.liverpool.ac.uk/adfs/discovery/keys\n    status: 200\n    note: One RSA signing key, 2,524 bytes.\n- name: entra-id-tenant\n  type: openIdConnect\n  description: >-\n    The institution's Microsoft Entra ID tenant, discoverable by its own domain. Microsoft hosts it;\n    the tenant\
  \ is Liverpool's.\n  operator: federation\n  openIdConnectUrl: https://login.microsoftonline.com/liverpool.ac.uk/v2.0/.well-known/openid-configuration\n  issuer: https://login.microsoftonline.com/53255131-b129-4010-86e1-474bfd7e8076/v2.0\n  tenant_region_scope: EU\n  probes:\n  - url: https://login.microsoftonline.com/liverpool.ac.uk/v2.0/.well-known/openid-configuration\n    status: 200\n- name: shibboleth-saml2\n  type: saml2\n  description: >-\n    Institution-operated Shibboleth SAML 2.0 identity provider, published in the UK Access Management\n    Federation and self-published on its own host.\n  operator: federation\n  entity_id: urn:mace:eduserv.org.uk:athens:provider:liv.ac.uk\n  scope: liv.ac.uk\n  metadata_urls:\n  - http://mdq.ukfederation.org.uk/entities/urn%3Amace%3Aeduserv.org.uk%3Aathens%3Aprovider%3Aliv.ac.uk\n  - https://shibboleth3.liv.ac.uk/idp/shibboleth\n  bindings:\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n\
  \  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign\n  probes:\n  - url: http://mdq.ukfederation.org.uk/entities/urn%3Amace%3Aeduserv.org.uk%3Aathens%3Aprovider%3Aliv.ac.uk\n    status: 200\n  - url: https://shibboleth3.liv.ac.uk/idp/shibboleth\n    status: 200\n  - url: https://shibboleth3.liv.ac.uk/idp/profile/SAML2/Redirect/SSO\n    status: 400\n    note: Live IdP rejecting a parameterless AuthnRequest.\n- name: adfs-saml2\n  type: saml2\n  description: AD FS SAML 2.0 / WS-Federation metadata for the institution's primary SP-initiated login.\n  operator: institution\n  entity_id: http://fs.liverpool.ac.uk/adfs/services/trust\n  metadata_urls:\n  - https://fs.liverpool.ac.uk/FederationMetadata/2007-06/FederationMetadata.xml\n  sso_location: https://fs.liverpool.ac.uk/adfs/ls/\n  probes:\n  - url: https://fs.liverpool.ac.uk/FederationMetadata/2007-06/FederationMetadata.xml\n    status: 200\n    note: 83,212 bytes, application/samlmetadata+xml.\ngated_surfaces:\n- url: https://canvas.liverpool.ac.uk/api/v1/accounts\n\
  \  status: 401\n  operator: tenant\n  note: Instructure Canvas data API on the institution's VLE host — token required, no public program.\n- url: https://elements.liverpool.ac.uk/\n  status: 401\n  operator: tenant\n  note: Symplectic Elements CRIS — HTTP auth challenge on the landing page itself.\n- url: https://datacat.liverpool.ac.uk/rest/eprint/2481.xml\n  status: 401\n  operator: institution\n  note: >-\n    DataCat's EPrints REST item fetch requires auth even though the same REST root and the OAI-PMH\n    interface are open — the two EPrints deployments are configured differently.\n- url: https://news.liverpool.ac.uk/wp-json/wp/v2/posts\n  status: 401\n  operator: institution\n  note: >-\n    The institution's WordPress newsroom deliberately gates the WP REST API; the RSS feed at\n    https://news.liverpool.ac.uk/feed/ (200, application/rss+xml, 205,842 bytes) is the open surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-liverpool/refs/heads/main/authentication/university-of-liverpool-authentication.yml
summary_line: none/oauth2/openIdConnect/saml2 · 5 schemes
tags:
- Education
- Higher Education
- University
- Russell Group
- United Kingdom
- Research
- Research Repository
- Research Data
- Open Access
- OAI-PMH
- EPrints
- Identity Federation
- Library
- Metadata
---
