---
api_key_in: []
api_specs:
- filename: victoria-university-of-wellington-website-globalobject-openapi.yml
  format: yaml
  label: Website Global Object
  slug: website-global-object
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/victoria-university-of-wellington/refs/heads/main/openapi/victoria-university-of-wellington-website-globalobject-openapi.yml
- filename: victoria-university-of-wellington-identity-federation-openapi.yml
  format: yaml
  label: Shibboleth Identity Provider (Tuakiri / eduGAIN)
  slug: identity-federation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/victoria-university-of-wellington/refs/heads/main/openapi/victoria-university-of-wellington-identity-federation-openapi.yml
- filename: victoria-university-of-wellington-institutional-repository-openapi.yml
  format: yaml
  label: Institutional Repository (self-hosted DSpace)
  slug: institutional-repository
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/victoria-university-of-wellington/refs/heads/main/openapi/victoria-university-of-wellington-institutional-repository-openapi.yml
auth_types: []
description: Authentication posture across Te Herenga Waka—Victoria University of Wellington's programmable surfaces. The institution issues no API keys and operates no developer portal, so there is nothing to register for. Every surface is either fully open or gated behind institutional identity — there is no middle tier.
kind: authentication
layout: security
method: derived
name: Victoria University Of Wellington Authentication
name_suffix: Authentication
oauth_flows: []
overview: Victoria University of Wellington declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Victoria University of Wellington
provider_slug: victoria-university-of-wellington
scheme_count: 0
schemes: []
slug: victoria-university-of-wellington-authentication
source_filename: victoria-university-of-wellington-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Victoria University of Wellington\nproviderId: victoria-university-of-wellington\ngenerated: '2026-08-30'\nmethod: derived\nprobe_date: '2026-08-30'\nprobe_note: >-\n  Written by API Evangelist from live, unauthenticated probes. Every status code and payload\n  quoted below was observed on the date above; nothing here was published by the institution.\nsource: live unauthenticated probes of every host in apis.yml, 2026-08-30\ndescription: >-\n  Authentication posture across Te Herenga Waka—Victoria University of Wellington's programmable\n  surfaces. The institution issues no API keys and operates no developer portal, so there is nothing\n  to register for. Every surface is either fully open or gated behind institutional identity — there\n  is no middle tier.\nsurfaces:\n- name: Website Global Object\n  operator: institution\n  url: https://www.wgtn.ac.nz/api/globalobject\n  scheme: none\n  detail:\
  \ >-\n    No authentication. HTTP 200 to an anonymous GET. Response carries\n    Access-Control-Allow-Origin \"*\" and Access-Control-Allow-Methods \"GET, HEAD, OPTIONS\", so it is\n    callable directly from a browser on any origin. No API key, no bearer token, no rate-limit\n    header observed.\n- name: Institutional repository — OAI-PMH, OpenSearch, Signposting\n  operator: institution\n  url: https://ir.wgtn.ac.nz/oai/request\n  scheme: none\n  detail: >-\n    No authentication and no key. The university's self-hosted DSpace 7.6.7 at ir.wgtn.ac.nz serves\n    its OAI-PMH 2.0 base URL, its OpenSearch 1.1 description and Atom result feed, and its FAIR\n    Signposting link sets to any anonymous caller — all returned HTTP 200 on 2026-08-30. This is the\n    only keyless, institution-operated bulk-data interface the university has, and it is\n    substantial: 23,150 records in twelve metadata formats.\n- name: Institutional repository — DSpace REST\n  operator: institution\n  url: https://ir.wgtn.ac.nz/server/api\n\
  \  scheme: bearer\n  detail: >-\n    SPLIT SURFACE. The HAL root, /server/api/core/communities, /server/api/core/collections and\n    /server/api/discover/search/objects all answer anonymously with HTTP 200. Item enumeration does\n    not: /server/api/core/items returns HTTP 401 {\"status\":401,\"error\":\"Unauthorized\",\"message\":\n    \"Authentication is required\"}. The credential is a DSpace JWT from /server/api/authn/login tied\n    to an EPerson account issued by Library Systems — not self-service, and not purchasable.\n- name: Shibboleth Identity Provider metadata\n  operator: institution\n  url: https://idp.vuw.ac.nz/idp/shibboleth\n  scheme: none\n  detail: >-\n    Metadata retrieval is unauthenticated by design — SAML metadata must be publicly readable for\n    federation to work. The SSO endpoints behind it are not open: an unbound request to\n    /idp/profile/SAML2/Redirect/SSO returns HTTP 400, and a valid flow requires a signed\n    AuthnRequest from a service provider\
  \ registered in Tuakiri.\n- name: Library discovery SRU\n  operator: tenant\n  url: https://tewaharoa.victoria.ac.nz/view/sru/64VUW_INST\n  scheme: none\n  detail: >-\n    Ex Libris Primo/Alma SRU 1.2 on the institution's own subdomain. Keyless: an anonymous\n    searchRetrieve returned HTTP 200 and 20,136 matching MARCXML records. This is the most\n    substantial anonymously callable interface associated with the institution, and the contract\n    behind it is Ex Libris's.\n- name: Open Access repository\n  operator: tenant\n  url: https://openaccess.wgtn.ac.nz/\n  scheme: none\n  detail: >-\n    Public repository, but the AWS WAF in front of it answers an anonymous non-browser request with\n    HTTP 202 and header x-amzn-waf-action \"challenge\" — a JavaScript bot challenge, not a\n    credential requirement. Live and bot-gated, not dead and not authenticated.\n- name: Nuku learning management (Canvas)\n  operator: tenant\n  url: https://nuku.wgtn.ac.nz/api/v1\n  scheme: oauth2\n  detail:\
  \ >-\n    Instructure Canvas REST API. Anonymous call returns HTTP 401\n    {\"status\":\"unauthenticated\",\"errors\":[{\"message\":\"user authorisation required\"}]}. Access\n    requires a Canvas OAuth2 token issued to a VUW account; browser sign-on federates to the\n    university's Microsoft Entra ID tenant.\n- name: Symplectic Elements research information system\n  operator: tenant\n  url: https://elements.wgtn.ac.nz/\n  scheme: institutional\n  detail: >-\n    HTTP 401 to an anonymous request. Host CNAMEs to vuw.elements.symplectic.org. The Elements API\n    is available to the institution under its Symplectic contract but is not public.\n- name: Enterprise single sign-on (WSO2 Identity Server)\n  operator: institution\n  url: https://auth-eis.vuw.ac.nz/\n  scheme: saml\n  detail: >-\n    Self-hosted WSO2 Identity Server, resolving directly to 130.195.13.55 with no CNAME. It is the\n    SAML issuer behind studentrecords.vuw.ac.nz, reached at /samlsso with a signed SAMLRequest and\n\
  \    RelayState /c/auth/SSB. Every discovery endpoint WSO2 normally publishes returns HTTP 403 from a\n    web application firewall that echoes a signature ID and the caller's IP — live and protected,\n    not missing.\n\n- name: Student records (Ellucian Banner Self-Service)\n  operator: tenant\n  url: https://studentrecords.vuw.ac.nz/\n  scheme: saml\n  detail: >-\n    HTTP 200 only after a redirect into the WSO2 SAML flow. No anonymous read, no public API, no\n    documented interface. Self-hosted on institution infrastructure (130.195.15.120, no CNAME); the\n    contract remains Ellucian's.\n\n- name: Microsoft Entra ID tenant\n  operator: tenant\n  url: https://login.microsoftonline.com/cfe63e23-6951-427e-8683-bb84dcf1d20c/v2.0/.well-known/openid-configuration\n  scheme: oidc\n  detail: >-\n    OpenID Connect discovery document for the university's Entra ID tenant returns HTTP 200\n    anonymously, as does the WS-Federation/SAML federationmetadata document. Discovery is open;\n  \
  \  every token endpoint behind it requires a registered client.\nnotes: >-\n  No institution-issued API credential of any kind was found. Nothing here is purchasable, and\n  nothing here is self-service.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/victoria-university-of-wellington/refs/heads/main/authentication/victoria-university-of-wellington-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- New Zealand
- Public Research University
- Research
- Open Access
- Research Repository
- Institutional Repository
- OAI-PMH
- DSpace
- Library
- Course Catalog
- Identity Federation
- Research Computing
---
