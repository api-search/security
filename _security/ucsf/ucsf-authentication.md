---
api_key_in: []
api_specs:
- filename: ucsf-profiles-json-openapi.yml
  format: yaml
  label: UCSF Profiles JSON API
  slug: profiles-json
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsf/refs/heads/main/openapi/ucsf-profiles-json-openapi.yml
- filename: ucsf-industry-documents-solr-openapi.yml
  format: yaml
  label: UCSF Industry Documents Library Solr API
  slug: industry-documents-solr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsf/refs/heads/main/openapi/ucsf-industry-documents-solr-openapi.yml
auth_types: []
description: Authentication posture across every institution-operated UCSF surface API Evangelist was able to reach and verify from the public internet.
kind: authentication
layout: security
method: probed
name: Ucsf Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of California, San Francisco declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of California, San Francisco
provider_slug: ucsf
scheme_count: 0
schemes: []
slug: ucsf-authentication
source_filename: ucsf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: UCSF Authentication\ndescription: >-\n  Authentication posture across every institution-operated UCSF surface API Evangelist was able\n  to reach and verify from the public internet.\ngenerated: '2026-08-19'\nmethod: probed\nsource:\n  - https://profilesdeveloper.ucsf.edu/json-api\n  - https://solr.idl.ucsf.edu/solr/ltdl3/query?q=*:*&rows=0&wt=json\n  - https://mdq.incommon.org/entities/urn%3Amace%3Aincommon%3Aucsf.edu\nsurfaces:\n  - api: UCSF Profiles JSON API\n    x-operator: institution\n    baseURL: https://api.profiles.ucsf.edu/json/v2/\n    scheme: none\n    keys_required: false\n    notes: >-\n      No credential of any kind. A `source` query parameter identifying the calling application\n      is required, but it is an attribution/courtesy identifier, not a secret and not verified —\n      it is not an API key. UCSF asks callers to make contact before production use, to add an\n      acknowledgement, to refresh cached data weekly, and to leave at least one second\
  \ between\n      calls. Those are stated conditions of use, not enforced controls.\n    verified: '2026-08-19'\n    verified_status: 200\n  - api: UCSF Industry Documents Library Solr API\n    x-operator: institution\n    baseURL: https://solr.idl.ucsf.edu/solr/ltdl3\n    scheme: none\n    keys_required: false\n    notes: >-\n      Fully anonymous read access to the ltdl3 collection. Only the documented collection is\n      exposed; sibling Solr collection names return 403.\n    verified: '2026-08-19'\n    verified_status: 200\n  - api: UCSF Identity Provider (Shibboleth / InCommon)\n    x-operator: institution\n    entityID: urn:mace:incommon:ucsf.edu\n    metadata: https://dp.ucsf.edu/idp/shibboleth\n    metadata_federated: https://mdq.incommon.org/entities/urn%3Amace%3Aincommon%3Aucsf.edu\n    scheme: saml2\n    protocols:\n      - urn:oasis:names:tc:SAML:2.0:protocol\n      - urn:oasis:names:tc:SAML:1.1:protocol\n      - urn:mace:shibboleth:1.0\n    endpoints:\n      SingleSignOnService:\n\
  \        - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n          location: https://dp.ucsf.edu/idp/profile/SAML2/Redirect/SSO\n        - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n          location: https://dp.ucsf.edu/idp/profile/SAML2/POST/SSO\n        - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign\n          location: https://dp.ucsf.edu/idp/profile/SAML2/POST-SimpleSign/SSO\n        - binding: urn:mace:shibboleth:1.0:profiles:AuthnRequest\n          location: https://dp.ucsf.edu/idp/profile/Shibboleth/SSO\n      SingleLogoutService:\n        - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n          location: https://dp.ucsf.edu/idp/profile/SAML2/Redirect/SLO\n        - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n          location: https://dp.ucsf.edu/idp/profile/SAML2/POST/SLO\n    notes: >-\n      UCSF operates its own Shibboleth Identity Provider and registers it in the InCommon\n      Federation,\
  \ which is re-exported to eduGAIN. This is machine-readable, signed, publicly\n      retrievable federation metadata and it is unambiguously institution-operated. A local copy\n      of the signed metadata retrieved on 2026-08-19 is stored alongside this file as\n      ucsf-incommon-saml-metadata.xml, alongside UCSF's own first-party copy retrieved from\n      https://dp.ucsf.edu/idp/shibboleth as ucsf-idp-self-published-metadata.xml — an EntitiesDescriptor\n      named https://ucsf-federation.edu/metadata/myaccess-ucsf.xml carrying an IDPSSODescriptor, an\n      AttributeAuthorityDescriptor, an SPSSODescriptor and shibmd:Scope ucsf.edu. UCSF separately fronts interactive login with Okta at\n      login.ucsf.edu; the federated SAML entity remains dp.ucsf.edu.\n    verified: '2026-08-19'\n    verified_status: 200\ngated:\n  - host: unified-api.ucsf.edu\n    x-operator: institution\n    observed_status: 403\n    notes: >-\n      Live host under ucsf.edu fronted by a Citrix NetScaler JavaScript\
  \ challenge. No public\n      documentation for it was located, so no surface is claimed from it. Recorded as evidence\n      that UCSF runs an API gateway, not as a consumable API.\n    verified: '2026-08-19'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucsf/refs/heads/main/authentication/ucsf-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- United States
- California
- UC System
- Public Research University
- Health Sciences
- Research
- Researcher Profiles
- Research Data
- Open Data
- Library
- Digital Archive
- Identity Federation
- Research Computing
---
