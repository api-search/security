---
api_key_in: []
api_specs:
- filename: iit-delhi-site-platform-openapi.yml
  format: yaml
  label: IIT Delhi Departmental Site Platform API
  slug: site-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iit-delhi/refs/heads/main/openapi/iit-delhi-site-platform-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Iit Delhi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Indian Institute of Technology Delhi declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Indian Institute of Technology Delhi
provider_slug: iit-delhi
scheme_count: 0
schemes: []
slug: iit-delhi-authentication
source_filename: iit-delhi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nname: IIT Delhi — authentication surfaces\ngenerated: '2026-08-30'\nmethod: derived\nx-derivation: probed\nsource:\n  - https://oauth.iitd.ac.in/\n  - https://oauth.iitd.ac.in/.well-known/openid-configuration\n  - https://oauth.iitd.ac.in/.well-known/oauth-authorization-server\n  - https://idp.iitd.ac.in/idp/shibboleth\n  - https://convocation.iitd.ac.in/api/gallery\n  - https://ir.iitd.ac.in/server/api\n  - https://ir.iitd.ac.in/server/api/core/items\nnote: >-\n  Every statement below was observed on 2026-08-30 against a live host. IIT Delhi\n  publishes no developer-facing authentication documentation of any kind; what is\n  recorded here is behaviour, not a documented contract.\n\nmechanisms:\n  - id: shibboleth-saml2\n    label: Shibboleth SAML 2.0 identity provider\n    x-operator: institution\n    status: live\n    entity_id: https://idp.iitd.ac.in/idp/shibboleth\n    metadata_url: https://idp.iitd.ac.in/idp/shibboleth\n    scope: iitd.ac.in\n    federation:\n  \
  \    name: INFED — Indian Access Management Federation\n      registration_authority: http://inflibnet.ac.in\n      interfederated_via: eduGAIN\n      edugain_entity_id: '672721'\n      first_seen_in_edugain: '2020-03-28'\n      edugain_connectivity_check: passing\n    profiles_advertised:\n      - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect (SSO)\n      - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST (SSO)\n      - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign (SSO)\n      - urn:mace:shibboleth:1.0:profiles:AuthnRequest (SSO)\n      - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect (SLO)\n      - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST (SLO)\n      - urn:oasis:names:tc:SAML:2.0:bindings:SOAP (SLO, port 8443)\n      - urn:oasis:names:tc:SAML:2.0:bindings:SOAP (ArtifactResolution, port 8443)\n    roles:\n      - IDPSSODescriptor\n      - AttributeAuthorityDescriptor\n    evidence:\n      - url: https://idp.iitd.ac.in/idp/shibboleth\n        status: 200\n  \
  \      content_type: application/xml\n        detail: >-\n          14,514-byte SAML 2.0 EntityDescriptor, OrganizationName \"Indian Institute of\n          Technology Delhi\", shibmd:Scope iitd.ac.in.\n      - url: https://idp.iitd.ac.in/idp/profile/SAML2/Redirect/SSO\n        status: 400\n        detail: >-\n          Shibboleth \"Stale Request\" page — the correct response to an unsolicited GET,\n          and positive proof the SSO profile is running rather than parked.\n    assessment: >-\n      The single strongest machine-readable surface IIT Delhi operates. Institution-run\n      by definition, self-describing, federation-registered, and entirely uncatalogued\n      anywhere in the institute's own developer-facing material.\n\n  - id: iitd-oauth2\n    label: IIT Delhi OAuth 2 apps server\n    x-operator: institution\n    status: live-but-gated\n    portal: https://oauth.iitd.ac.in/\n    self_description: >-\n      \"Welcome to IIT Delhi's OAuth 2 apps server. You can create your\
  \ own apps and use\n      IIT Delhi's authentication too!\"\n    discovery:\n      openid_configuration: absent\n      oauth_authorization_server_metadata: absent\n      protected_resource_metadata: absent\n      dynamic_client_registration: not_published\n    published_scopes: none\n    evidence:\n      - url: https://oauth.iitd.ac.in/\n        status: 200\n        detail: Live portal, all detail behind an interactive login.\n      - url: https://oauth.iitd.ac.in/.well-known/openid-configuration\n        status: 404\n      - url: https://oauth.iitd.ac.in/.well-known/oauth-authorization-server\n        status: 404\n      - url: https://convocation.iitd.ac.in/api/gallery\n        status: 401\n        detail: >-\n          Cross-confirms the OAuth server is the real gate for institute web APIs — the\n          body reads \"Authentication required. Please login via IITD OAuth.\"\n    assessment: >-\n      A genuine institution-operated authorization server with a developer-registration\n\
  \      story, and no machine-readable description of it whatsoever. An agent or an outside\n      developer cannot discover an endpoint, a grant type or a scope. This is the single\n      highest-leverage fix available to IIT Delhi: publishing RFC 8414 metadata would cost\n      one static document.\n\n  - id: dspace-rest\n    label: DSpace 8 REST API session/JWT authentication\n    x-operator: institution\n    status: live\n    note: >-\n      Host is the institute's own; the contract is the DSpace product's, not IIT Delhi's,\n      so no DSpace spec is saved in this repo. Recorded here for the access boundary only.\n    anonymous_read: partial\n    evidence:\n      - url: https://ir.iitd.ac.in/server/api\n        status: 200\n        detail: Root HAL document public; advertises an `authn` link and dspaceVersion \"DSpace 8.0\".\n      - url: https://ir.iitd.ac.in/server/api/discover/search/objects?query=api\n        status: 200\n        detail: Discovery search answers anonymously and\
  \ returns embedded results.\n      - url: https://ir.iitd.ac.in/server/api/core/items\n        status: 401\n        detail: '{\"status\":401,\"error\":\"Unauthorized\",\"message\":\"Authentication is required\"}'\n\nfindings:\n  - severity: medium\n    id: session-id-in-401-body\n    detail: >-\n      convocation.iitd.ac.in returns a `debug` object containing a live `sessionID` to\n      wholly unauthenticated callers on the 401 path. Diagnostics of this kind belong in\n      server logs, never in an anonymous response body.\n    evidence:\n      - url: https://convocation.iitd.ac.in/api/gallery\n        status: 401\n  - severity: medium\n    id: no-authorization-server-metadata\n    detail: >-\n      The institute runs an OAuth 2 authorization server and publishes neither OpenID\n      Connect discovery nor RFC 8414 metadata, so nothing about it is machine-readable.\n    evidence:\n      - url: https://oauth.iitd.ac.in/.well-known/openid-configuration\n        status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iit-delhi/refs/heads/main/authentication/iit-delhi-authentication.yml
summary_line: 0 schemes
tags:
- Education
- Higher Education
- University
- Institute of Technology
- Research
- India
- Open Access
- Library
- Research Repository
- Identity Federation
---
