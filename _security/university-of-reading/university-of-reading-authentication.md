---
api_key_in: []
api_specs:
- filename: university-of-reading-centaur-oai-pmh-openapi.yml
  format: yaml
  label: CentAUR OAI-PMH Metadata API
  slug: centaur-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-reading/refs/heads/main/openapi/university-of-reading-centaur-oai-pmh-openapi.yml
- filename: university-of-reading-research-data-archive-oai-pmh-openapi.yml
  format: yaml
  label: Research Data Archive OAI-PMH Metadata API
  slug: research-data-archive-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-reading/refs/heads/main/openapi/university-of-reading-research-data-archive-oai-pmh-openapi.yml
- filename: university-of-reading-eprints-rest-openapi.yml
  format: yaml
  label: CentAUR Repository REST Listings
  slug: centaur-eprints-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-reading/refs/heads/main/openapi/university-of-reading-eprints-rest-openapi.yml
- filename: university-of-reading-eprints-rest-openapi.yml
  format: yaml
  label: Research Data Archive REST Listings
  slug: research-data-archive-eprints-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-reading/refs/heads/main/openapi/university-of-reading-eprints-rest-openapi.yml
auth_types:
- none
- saml2
- oidc
description: ''
kind: authentication
layout: security
method: derived
name: University Of Reading Authentication
name_suffix: Authentication
oauth_flows:
- authorization_code
overview: University of Reading secures its APIs with none, saml2, and oidc across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorization_code flow(s).
provider_name: University of Reading
provider_slug: university-of-reading
scheme_count: 4
schemes:
- applies_to:
  - https://centaur.reading.ac.uk/cgi/oai2
  - https://researchdata.reading.ac.uk/cgi/oai2
  - https://centaur.reading.ac.uk/rest/
  - https://researchdata.reading.ac.uk/rest/
  description: Fully open. Every OAI-PMH verb was exercised with no credentials and no session, and the /rest/ dataset listings returned 200 the same way. No API key, no registration, no Authorization header, and no advertised rate limit or quota.
  name: none
  purpose: OAI-PMH harvesting and the read-only repository dataset listings.
  sources:
  - openapi/university-of-reading-centaur-oai-pmh-openapi.yml
  - openapi/university-of-reading-eprints-rest-openapi.yml
  type: none
- applies_to:
  - https://centaur.reading.ac.uk/rest/eprint/{id}.xml
  - https://researchdata.reading.ac.uk/rest/eprint/{id}.xml
  description: 'GET of a per-record XML document returned 401 with an "EPrints REST: Auth Required" body on both hosts. EPrints authenticates these with a repository user account. No public route to obtain one was found — accounts are for depositors and staff. The open substitute is OAI-PMH, which serves the same metadata without credentials.'
  issuance: Not publicly issuable. Repository accounts are institutional.
  name: eprints-rest-record-auth
  purpose: Retrieving an individual repository record as EPrints XML.
  sources:
  - openapi/university-of-reading-eprints-rest-openapi.yml
  type: http
- applies_to:
  - https://reading.ac.uk/oala/metadata
  description: The university's identity provider entity in the UK Access Management Federation, entityID https://reading.ac.uk/oala/metadata, scoped to reading.ac.uk and reading.edu.my. Metadata is published by the federation's MDQ service; the SSO endpoints resolve to OpenAthens (https://login.openathens.net/saml/2/sso/reading.ac.uk/c/ukfed), which is the implementation the university has chosen. Both SAML 2.0 and the Shibboleth 1.0 AuthnRequest profile are advertised.
  issuance: Institutional accounts only; a federation entity is not a developer credential.
  name: uk-federation-saml
  purpose: Federated sign-in to externally hosted licensed resources — library discovery, publisher platforms, and other UK federation / eduGAIN service providers.
  sources:
  - http://mdq.ukfederation.org.uk/entities/%7Bsha1%7D57cf958ecb2c90e4fb339c8cf8a95dcee2d68101
  type: saml2
- applies_to:
  - https://timetable.reading.ac.uk/
  - https://myid.reading.ac.uk/
  - https://risis.reading.ac.uk/
  description: Microsoft Entra ID tenant 4ffa3bc4-ecfc-48c0-9080-f5e43ff90e5f. The discovery document at https://login.microsoftonline.com/reading.ac.uk/v2.0/.well-known/openid-configuration is public and complete (authorization_code and implicit response types, scopes openid profile email offline_access, JWKS published). Probing timetable.reading.ac.uk and myid.reading.ac.uk each redirected into this tenant, confirming which applications sit behind it. The tenant is Managed — getuserrealm returns NameSpaceType Managed, FederationBrandName "University of Reading" — so there is no on-premises federation server behind it.
  issuance: 'Application registrations in this tenant are administered by the university. There is no self-service developer onboarding: an external party cannot obtain a client_id here.'
  name: entra-id-oidc
  purpose: Sign-in to the university's own web applications — timetabling, identity self-service, staff and student portals.
  sources:
  - https://login.microsoftonline.com/reading.ac.uk/v2.0/.well-known/openid-configuration
  type: oidc
slug: university-of-reading-authentication
source_filename: university-of-reading-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: derived\nsource: >-\n  Live unauthenticated probes of University of Reading hosts on 2026-09-01, plus the UK Access\n  Management Federation MDQ record and the institution's Entra ID OpenID Connect discovery\n  document.\nsummary:\n  types:\n  - none\n  - saml2\n  - oidc\n  api_key_in: []\n  oauth2_flows:\n  - authorization_code\n  note: >-\n    The University of Reading issues no API credential of any kind to the public. Its two open\n    machine-readable surfaces need no authentication at all, and everything else needs to BE a\n    member of the university: the institutional identity plane is a Microsoft Entra ID tenant for\n    internal applications and a UK federation SAML entity for external licensed resources. There is\n    no developer registration, no API key console, no client-credentials flow a third party can\n    enter, and no documented route by which an outside developer could obtain access to a\n    university system.\nschemes:\n\
  - name: none\n  type: none\n  purpose: OAI-PMH harvesting and the read-only repository dataset listings.\n  applies_to:\n  - https://centaur.reading.ac.uk/cgi/oai2\n  - https://researchdata.reading.ac.uk/cgi/oai2\n  - https://centaur.reading.ac.uk/rest/\n  - https://researchdata.reading.ac.uk/rest/\n  description: >-\n    Fully open. Every OAI-PMH verb was exercised with no credentials and no session, and the\n    /rest/ dataset listings returned 200 the same way. No API key, no registration, no Authorization\n    header, and no advertised rate limit or quota.\n  sources:\n  - openapi/university-of-reading-centaur-oai-pmh-openapi.yml\n  - openapi/university-of-reading-eprints-rest-openapi.yml\n- name: eprints-rest-record-auth\n  type: http\n  purpose: Retrieving an individual repository record as EPrints XML.\n  applies_to:\n  - https://centaur.reading.ac.uk/rest/eprint/{id}.xml\n  - https://researchdata.reading.ac.uk/rest/eprint/{id}.xml\n  description: >-\n    GET of a per-record XML\
  \ document returned 401 with an \"EPrints REST: Auth Required\" body on both\n    hosts. EPrints authenticates these with a repository user account. No public route to obtain one\n    was found — accounts are for depositors and staff. The open substitute is OAI-PMH, which serves\n    the same metadata without credentials.\n  issuance: Not publicly issuable. Repository accounts are institutional.\n  sources:\n  - openapi/university-of-reading-eprints-rest-openapi.yml\n- name: uk-federation-saml\n  type: saml2\n  purpose: >-\n    Federated sign-in to externally hosted licensed resources — library discovery, publisher\n    platforms, and other UK federation / eduGAIN service providers.\n  applies_to:\n  - https://reading.ac.uk/oala/metadata\n  description: >-\n    The university's identity provider entity in the UK Access Management Federation, entityID\n    https://reading.ac.uk/oala/metadata, scoped to reading.ac.uk and reading.edu.my. Metadata is\n    published by the federation's MDQ\
  \ service; the SSO endpoints resolve to OpenAthens\n    (https://login.openathens.net/saml/2/sso/reading.ac.uk/c/ukfed), which is the implementation the\n    university has chosen. Both SAML 2.0 and the Shibboleth 1.0 AuthnRequest profile are advertised.\n  issuance: Institutional accounts only; a federation entity is not a developer credential.\n  sources:\n  - http://mdq.ukfederation.org.uk/entities/%7Bsha1%7D57cf958ecb2c90e4fb339c8cf8a95dcee2d68101\n- name: entra-id-oidc\n  type: oidc\n  purpose: Sign-in to the university's own web applications — timetabling, identity self-service, staff and student portals.\n  applies_to:\n  - https://timetable.reading.ac.uk/\n  - https://myid.reading.ac.uk/\n  - https://risis.reading.ac.uk/\n  description: >-\n    Microsoft Entra ID tenant 4ffa3bc4-ecfc-48c0-9080-f5e43ff90e5f. The discovery document at\n    https://login.microsoftonline.com/reading.ac.uk/v2.0/.well-known/openid-configuration is public\n    and complete (authorization_code and implicit\
  \ response types, scopes openid profile email\n    offline_access, JWKS published). Probing timetable.reading.ac.uk and myid.reading.ac.uk each\n    redirected into this tenant, confirming which applications sit behind it. The tenant is\n    Managed — getuserrealm returns NameSpaceType Managed, FederationBrandName \"University of\n    Reading\" — so there is no on-premises federation server behind it.\n  issuance: >-\n    Application registrations in this tenant are administered by the university. There is no\n    self-service developer onboarding: an external party cannot obtain a client_id here.\n  sources:\n  - https://login.microsoftonline.com/reading.ac.uk/v2.0/.well-known/openid-configuration\nobservations:\n- >-\n  A bot challenge, not an auth wall, guards part of the repository. /cgi/search and /cgi/export on\n  centaur.reading.ac.uk return HTTP 200 carrying an Anubis interstitial (\"Making sure you're not a\n  bot!\") instead of the requested document. It is not authentication\
  \ and it does not affect\n  /cgi/oai2 or /rest/, but a naive harvester reading status codes alone would record those paths as\n  successful.\n- >-\n  An Azure API Management gateway runs on the institution's own domain — esb-prod-api.reading.ac.uk\n  resolves to uks-common-p-001-apim.azure-api.net, with a UAT sibling at esb-uat-api.reading.ac.uk.\n  Both answer with APIM's JSON 404 envelope on every path probed. The university therefore operates\n  an API gateway; it publishes no route through it, and no subscription-key issuance process is\n  public.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-reading/refs/heads/main/authentication/university-of-reading-authentication.yml
summary_line: none/saml2/oidc · 4 schemes
tags:
- University
- Higher Education
- Education
- Research
- Research Repository
- Research Data
- Open Access
- OAI-PMH
- Metadata
- Identity Federation
- Course Catalog
- Library
- Climate Data
- United Kingdom
- England
---
