---
api_key_in: []
api_specs:
- filename: university-of-southampton-open-data-linked-data-openapi.yml
  format: yaml
  label: University of Southampton Open Data Service (Linked Data)
  slug: open-data-linked-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-southampton/refs/heads/main/openapi/university-of-southampton-open-data-linked-data-openapi.yml
- filename: university-of-southampton-eprints-oai-pmh-openapi.yml
  format: yaml
  label: ePrints Soton OAI-PMH Interface
  slug: eprints-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-southampton/refs/heads/main/openapi/university-of-southampton-eprints-oai-pmh-openapi.yml
- filename: university-of-southampton-eprints-rest-openapi.yml
  format: yaml
  label: ePrints Soton REST Interface
  slug: eprints-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-southampton/refs/heads/main/openapi/university-of-southampton-eprints-rest-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: University Of Southampton Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Southampton declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Southampton
provider_slug: university-of-southampton
scheme_count: 0
schemes: []
slug: university-of-southampton-authentication
source_filename: university-of-southampton-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\ngenerated: '2026-08-30'\nmethod: probed\nsource: >-\n  Live retrieval of the University's Shibboleth IdP metadata on 2026-08-30, from both the IdP's own\n  publication point (https://webauth.soton.ac.uk/idp/shibboleth, 200, application/xml, 16951 bytes)\n  and the Jisc UK Access Management Federation MDQ service\n  (http://mdq.ukfederation.org.uk/entities/https%3A%2F%2Fwebauth.soton.ac.uk%2Fshibboleth, 200,\n  application/samlmetadata+xml, 19396 bytes). The federation copy is signed and is saved as\n  authentication/university-of-southampton-saml-idp-metadata.xml. Endpoint bindings below were read\n  out of that document, not assumed from the Shibboleth defaults.\n\nsummary: >-\n  The University of Southampton's public programmable surfaces are unauthenticated. The Open Data\n  Service, the ePrints OAI-PMH interface and the ePrints REST interface all require no key, no\n  token and no account. The University's authentication apparatus is federated identity for\n  consuming\
  \ licensed resources and internal systems, not an API gateway — and the SAML Identity\n  Provider is itself the most substantial machine-readable artifact the institution operates.\n\nauthentication:\n\n- surface: Open Data Service (data.southampton.ac.uk / id.southampton.ac.uk)\n  x-operator: institution\n  scheme: none\n  detail: >-\n    Open, anonymous HTTP. No key, no registration, no rate-limit header observed. Licensed under\n    the Open Government Licence.\n  evidence:\n  - location: https://data.southampton.ac.uk/building/94A.ttl\n    status: 200\n    detail: Anonymous request returned 2329 bytes of text/turtle.\n\n- surface: ePrints Soton OAI-PMH (eprints.soton.ac.uk/cgi/oai2)\n  x-operator: institution\n  scheme: none\n  detail: >-\n    Open, anonymous OAI-PMH. No key. Access is however gated by an Anubis proof-of-work bot\n    challenge that keys off User-Agent rather than credentials: a browser-like User-Agent receives\n    HTTP 401 with a challenge page and Googlebot receives\
  \ HTTP 403, while a plain or harvester\n    User-Agent is served normally with HTTP 200. This is anti-scraping, not authentication, but a\n    client must handle it to reach the data.\n  evidence:\n  - location: https://eprints.soton.ac.uk/cgi/oai2?verb=Identify\n    status: 200\n    detail: Retrieved with User-Agent \"OAIHarvester/2.0\"; valid OAI-PMH envelope, 4614 bytes.\n  - location: https://eprints.soton.ac.uk/cgi/oai2?verb=Identify\n    status: 401\n    detail: Same URL with a Chrome User-Agent; Anubis 1.24.0 challenge page, techaro.lol cookies set.\n\n- surface: ePrints Soton REST (eprints.soton.ac.uk/rest)\n  x-operator: institution\n  scheme: none\n  detail: Open, anonymous read. Same Anubis User-Agent gate as the OAI-PMH surface.\n  evidence:\n  - location: https://eprints.soton.ac.uk/rest/eprint/498754.xml\n    status: 200\n    detail: Anonymous request returned 5106 bytes of EPrints XML.\n\n- surface: Shibboleth SAML 2.0 Identity Provider\n  x-operator: institution\n  scheme:\
  \ saml\n  entity_id: https://webauth.soton.ac.uk/shibboleth\n  scope: soton.ac.uk\n  software: Shibboleth 3.x IdP\n  federation: Jisc UK Access Management Federation, onward to eduGAIN\n  detail: >-\n    The University's own IdP, self-declared in metadata as \"Shibboleth 3.x IdP for University of\n    Southampton\" with OrganizationName \"University of Southampton\" and shibmd:Scope \"soton.ac.uk\".\n    It carries IDPSSODescriptor, AttributeAuthorityDescriptor and SPSSODescriptor roles, and\n    advertises SAML 2.0, SAML 1.1 and the native urn:mace:shibboleth:1.0 authn profile. This is\n    federated single sign-on, not a developer API: an application cannot obtain an assertion\n    without first being registered as a service provider in the federation.\n  protocols:\n  - urn:oasis:names:tc:SAML:2.0:protocol\n  - urn:oasis:names:tc:SAML:1.1:protocol\n  - urn:mace:shibboleth:1.0\n  endpoints:\n  - binding: HTTP-Redirect\n    purpose: SingleSignOn\n    location: https://webauth.soton.ac.uk/idp/profile/SAML2/Redirect/SSO\n\
  \  - binding: HTTP-POST\n    purpose: SingleSignOn\n    location: https://webauth.soton.ac.uk/idp/profile/SAML2/POST/SSO\n  - binding: HTTP-POST-SimpleSign\n    purpose: SingleSignOn\n    location: https://webauth.soton.ac.uk/idp/profile/SAML2/POST-SimpleSign/SSO\n  - binding: Shibboleth authn request\n    purpose: SingleSignOn\n    location: https://webauth.soton.ac.uk/idp/profile/Shibboleth/SSO\n  - binding: HTTP-Redirect\n    purpose: SingleLogout\n    location: https://webauth.soton.ac.uk/idp/profile/SAML2/Redirect/SLO\n  - binding: SOAP\n    purpose: AttributeQuery\n    location: https://webauth.soton.ac.uk:8443/idp/profile/SAML2/SOAP/AttributeQuery\n  - binding: SOAP\n    purpose: ArtifactResolution\n    location: https://webauth.soton.ac.uk:8443/idp/profile/SAML2/SOAP/ArtifactResolution\n  evidence:\n  - location: https://webauth.soton.ac.uk/idp/shibboleth\n    status: 200\n    detail: >-\n      Unsigned EntityDescriptor published by the IdP itself, application/xml, 16951 bytes.\n\
  \  - location: http://mdq.ukfederation.org.uk/entities/https%3A%2F%2Fwebauth.soton.ac.uk%2Fshibboleth\n    status: 200\n    detail: >-\n      Signed EntityDescriptor from the UK federation MDQ service,\n      application/samlmetadata+xml, 19396 bytes. Saved to this repo.\n  - location: https://webauth.soton.ac.uk/idp/status\n    status: 403\n    detail: IdP status handler is access-controlled, as expected for a production deployment.\n\n- surface: Elsevier Pure CRIS tenancy (pure.soton.ac.uk)\n  x-operator: tenant\n  scheme: saml\n  detail: >-\n    Fronted by Microsoft Entra ID for the University's own tenant\n    (4a5378f9-29f4-4d3e-be89-669d03ada9d8). The Pure web services are not publicly reachable:\n    /ws/oai and /ws/api both return HTTP 403 from Elsevier's own error page. Southampton exposes no\n    public Pure API, unlike several peers in this cohort.\n  evidence:\n  - location: https://pure.soton.ac.uk/\n    status: 200\n    detail: Redirects to login.microsoftonline.com SAML2\
  \ sign-in for the University's Entra tenant.\n  - location: https://pure.soton.ac.uk/ws/oai?verb=Identify\n    status: 403\n    detail: Elsevier-branded 403 page. No public OAI-PMH on the Pure tenancy.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-southampton/refs/heads/main/authentication/university-of-southampton-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Russell Group
- United Kingdom
- Open Data
- Linked Data
- Research Repository
- Identity Federation
- OAI-PMH
- Research
- Course Catalog
---
