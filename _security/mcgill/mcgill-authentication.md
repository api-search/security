---
api_key_in: []
api_specs:
- filename: mcgill-shibboleth-idp-openapi.yml
  format: yaml
  label: McGill University Authentication Service — Shibboleth SAML 2.0 Identity Provider
  slug: shibboleth-idp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcgill/refs/heads/main/openapi/mcgill-shibboleth-idp-openapi.yml
auth_types:
- saml
- none
description: 'Authentication posture across McGill University''s machine-readable surfaces. McGill operates no API key programme and no OAuth authorization server of its own. Its one institution-operated authentication surface is a SAML 2.0 identity provider; every other reachable surface is either fully unauthenticated read-only metadata or an authenticated area of a platform McGill is a tenant on, where the credential is issued by the platform and not by McGill.


  This file replaces an earlier version that described an X-Dataverse-key API token as McGill''s authentication scheme. That token is Dataverse''s, issued by Borealis (Scholars Portal), and attributing it to McGill credited the institution with a vendor''s access-control design.'
kind: authentication
layout: security
method: probed
name: Mcgill Authentication
name_suffix: Authentication
oauth_flows: []
overview: McGill University secures its APIs with saml and none across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: McGill University
provider_slug: mcgill
scheme_count: 2
schemes:
- bindings:
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign
  description: SAML 2.0 web browser SSO against McGill's Shibboleth identity provider. Relying parties configure trust from the published metadata; there is no client-credential or machine-to-machine flow, and access is granted to registered service providers, not to arbitrary API clients.
  endpoints:
  - type: SingleSignOnService
    url: https://shibboleth.mcgill.ca/idp/profile/SAML2/Redirect/SSO
  - type: SingleSignOnService
    url: https://shibboleth.mcgill.ca/idp/profile/SAML2/POST/SSO
  - type: SingleLogoutService
    url: https://shibboleth.mcgill.ca/idp/profile/SAML2/Redirect/SLO
  entity_id: https://shibboleth.mcgill.ca/idp/shibboleth
  metadata_url: https://shibboleth.mcgill.ca/idp/shibboleth
  name: ShibbolethSAML
  operator: institution
  scope: mcgill.ca
  sources:
  - openapi/mcgill-shibboleth-idp-openapi.yml
  type: saml
- description: The SAML metadata document itself is served unauthenticated, as federation metadata must be. No credential, no rate-limit header, no registration.
  name: PublicMetadataAnonymous
  operator: institution
  sources:
  - openapi/mcgill-shibboleth-idp-openapi.yml
  type: none
slug: mcgill-authentication
source_filename: mcgill-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\ngenerated: '2026-08-30'\nmodified: '2026-08-30'\nmethod: probed\nsource: >-\n  https://shibboleth.mcgill.ca/idp/shibboleth (SAML 2.0 metadata, HTTP 200, 2026-08-30);\n  https://mcgill.scholaris.ca/server/api (DSpace REST root, HTTP 200, 2026-08-30);\n  https://mcgill.scholaris.ca/server/oai/request?verb=Identify (HTTP 200, 2026-08-30)\nprovider: McGill University\nproviderId: mcgill\ndescription: >-\n  Authentication posture across McGill University's machine-readable surfaces. McGill operates\n  no API key programme and no OAuth authorization server of its own. Its one institution-operated\n  authentication surface is a SAML 2.0 identity provider; every other reachable surface is either\n  fully unauthenticated read-only metadata or an authenticated area of a platform McGill is a\n  tenant on, where the credential is issued by the platform and not by McGill.\n\n\n  This file replaces an earlier version that described an X-Dataverse-key API token as McGill's\n  authentication\
  \ scheme. That token is Dataverse's, issued by Borealis (Scholars Portal), and\n  attributing it to McGill credited the institution with a vendor's access-control design.\nsummary:\n  types:\n  - saml\n  - none\n  api_key_programme: false\n  oauth_authorization_server: false\n  institution_operated_schemes: 1\nschemes:\n- name: ShibbolethSAML\n  type: saml\n  operator: institution\n  description: >-\n    SAML 2.0 web browser SSO against McGill's Shibboleth identity provider. Relying parties\n    configure trust from the published metadata; there is no client-credential or machine-to-machine\n    flow, and access is granted to registered service providers, not to arbitrary API clients.\n  entity_id: https://shibboleth.mcgill.ca/idp/shibboleth\n  metadata_url: https://shibboleth.mcgill.ca/idp/shibboleth\n  scope: mcgill.ca\n  bindings:\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign\n\
  \  endpoints:\n  - type: SingleSignOnService\n    url: https://shibboleth.mcgill.ca/idp/profile/SAML2/Redirect/SSO\n  - type: SingleSignOnService\n    url: https://shibboleth.mcgill.ca/idp/profile/SAML2/POST/SSO\n  - type: SingleLogoutService\n    url: https://shibboleth.mcgill.ca/idp/profile/SAML2/Redirect/SLO\n  sources:\n  - openapi/mcgill-shibboleth-idp-openapi.yml\n- name: PublicMetadataAnonymous\n  type: none\n  operator: institution\n  description: >-\n    The SAML metadata document itself is served unauthenticated, as federation metadata must be.\n    No credential, no rate-limit header, no registration.\n  sources:\n  - openapi/mcgill-shibboleth-idp-openapi.yml\ntenant_platform_schemes:\n- name: ScholarisAnonymousRead\n  type: none\n  operator: tenant\n  platform: Scholaris (Scholars Portal / OCUL) — DSpace 7\n  description: >-\n    eScholarship@McGill serves its DSpace REST (HAL) root and its OAI-PMH endpoint without\n    authentication for public read. Deposit and administration\
  \ are behind Scholaris accounts.\n    The scheme is DSpace's, not McGill's; recorded here as a tenant fact, not as McGill's design.\n  evidence:\n  - url: https://mcgill.scholaris.ca/server/api\n    status: 200\n  - url: https://mcgill.scholaris.ca/server/oai/request?verb=Identify\n    status: 200\n- name: BorealisDataverseToken\n  type: apiKey\n  operator: tenant\n  platform: Borealis (Scholars Portal / OCUL) — Dataverse\n  description: >-\n    The X-Dataverse-key header token governing write and private-data access to the McGill\n    University Dataverse. Issued by Borealis, defined by the Dataverse project, shared with every\n    other Borealis member institution. Recorded as the tenant relationship it is; NOT catalogued\n    as a McGill authentication scheme.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mcgill/refs/heads/main/authentication/mcgill-authentication.yml
summary_line: saml/none · 2 schemes
tags:
- University
- Higher Education
- Education
- Canada
- Quebec
- U15
- Public Research University
- Identity Federation
- Research Repository
- Research Data
- Course Catalog
---
