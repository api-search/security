---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Dtu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Technical University of Denmark declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Technical University of Denmark
provider_slug: dtu
scheme_count: 0
schemes: []
slug: dtu-authentication
source_filename: dtu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\n# DTU — institutional identity + authentication surface\n# x-operator: institution — every endpoint below is served from a host under\n# DTU's own registrable domain (dtu.dk) and is DTU's own deployment.\ngenerated: '2026-08-30'\nmethod: probed\nsource: >-\n  Live HTTP probes of https://sts.ait.dtu.dk/FederationMetadata/2007-06/FederationMetadata.xml\n  and https://sts.ait.dtu.dk/adfs/.well-known/openid-configuration, cross-checked against the\n  WAYF national federation IdP feed (https://metadata.wayf.dk/idps.js) and the eduGAIN feed\n  (https://phph.wayf.dk/md/idpsedugain.json).\nprovider: Technical University of Denmark\nproviderId: dtu\nx-operator: institution\n\nidentity_provider:\n  name: DTU Security Token Service (Microsoft AD FS)\n  entity_id: http://sts.ait.dtu.dk/adfs/services/trust\n  host: sts.ait.dtu.dk\n  service_display_name: Logon using DTU credentials\n  schac_home_organization: dtu.dk\n  scopes:\n  - dtu.dk\n  - guest.dtu.dk\n  federations:\n  - name:\
  \ WAYF (Where Are You From) — Danish national identity federation\n    url: https://www.wayf.dk/en\n    listed_as: Technical University of Denmark (DTU) / Danmarks Tekniske Universitet\n    evidence: https://metadata.wayf.dk/idps.js\n    status: 200\n  - name: eduGAIN (via WAYF)\n    evidence: https://phph.wayf.dk/md/idpsedugain.json\n    status: 200\n\nprotocols:\n- protocol: SAML 2.0\n  role: IDPSSODescriptor + SPSSODescriptor\n  metadata:\n    url: https://sts.ait.dtu.dk/FederationMetadata/2007-06/FederationMetadata.xml\n    status: 200\n    content_type: application/samlmetadata+xml\n    bytes: 71790\n    signed: true\n    signature_algorithm: http://www.w3.org/2001/04/xmldsig-more#rsa-sha256\n  endpoints:\n    single_sign_on:\n    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n      location: https://sts.ait.dtu.dk/adfs/ls/\n    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n      location: https://sts.ait.dtu.dk/adfs/ls/\n    single_logout:\n    - binding:\
  \ urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n      location: https://sts.ait.dtu.dk/adfs/ls/\n    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n      location: https://sts.ait.dtu.dk/adfs/ls/\n- protocol: WS-Federation / WS-Trust\n  role: fed:SecurityTokenServiceType + fed:ApplicationServiceType\n  protocol_support:\n  - http://docs.oasis-open.org/ws-sx/ws-trust/200512\n  - http://schemas.xmlsoap.org/ws/2005/02/trust\n  - http://docs.oasis-open.org/wsfed/federation/200706\n- protocol: OpenID Connect 1.0 / OAuth 2.0\n  discovery:\n    url: https://sts.ait.dtu.dk/adfs/.well-known/openid-configuration\n    status: 200\n    content_type: application/json\n  issuer: https://sts.ait.dtu.dk/adfs\n  authorization_endpoint: https://sts.ait.dtu.dk/adfs/oauth2/authorize/\n  token_endpoint: https://sts.ait.dtu.dk/adfs/oauth2/token/\n  userinfo_endpoint: https://sts.ait.dtu.dk/adfs/userinfo\n  jwks_uri: https://sts.ait.dtu.dk/adfs/discovery/keys\n  end_session_endpoint: https://sts.ait.dtu.dk/adfs/oauth2/logout\n\
  \  scopes_supported:\n  - openid\n  - profile\n  - email\n  - allatclaims\n  - aza\n  - user_impersonation\n  - logon_cert\n  - vpn_cert\n  - winhello_cert\n  id_token_signing_alg_values_supported:\n  - RS256\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  - windows_client_authentication\n\nsecondary:\n- name: login.dtu.dk\n  description: >-\n    DTU web sign-in front door. Redirects to Microsoft Entra ID tenant\n    f251f123-c9ce-448e-9277-34bb285911d9 for OIDC authorization. The redirect target is\n    login.microsoftonline.com — a vendor host — so only the dtu.dk front door is recorded here.\n  url: https://login.dtu.dk/\n  status: 200\n  x-operator: institution\n- name: auth.dtu.dk\n  description: DTU federated authentication host; redirects to /dtu. No SAML or OIDC metadata is served at this host (probed 404).\n  url: https://auth.dtu.dk/\n  status: 200\n  x-operator: institution\n\nnotes: >-\n  DTU operates its own\
  \ token service rather than consuming an identity platform under a vendor\n  hostname, which makes this the clearest institution-operated, machine-readable surface DTU\n  publishes. No client registration is open or self-service: obtaining a relying-party trust\n  requires institutional affiliation and a request to DTU AIT. Federation metadata itself is\n  public and unauthenticated.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dtu/refs/heads/main/authentication/dtu-authentication.yml
summary_line: 0 schemes
tags:
- Education
- Higher Education
- University
- Technical University
- Denmark
- Europe
- Identity Federation
- Research Data
- Library
- Course Catalog
- Wind Energy
---
