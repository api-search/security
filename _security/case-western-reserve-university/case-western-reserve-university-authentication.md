---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Case Western Reserve University Authentication
name_suffix: Authentication
oauth_flows: []
overview: Case Western Reserve University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Case Western Reserve University
provider_slug: case-western-reserve-university
scheme_count: 0
schemes: []
slug: case-western-reserve-university-authentication
source_filename: case-western-reserve-university-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\n# How access to Case Western Reserve University's programmable surfaces is actually established.\n# NOT an OAuth developer program: CWRU publishes no API keys and no third-party client registration.\nname: Case Western Reserve University — authentication and federated identity\nslug: case-western-reserve-university\ngenerated: '2026-09-01'\nmethod: probed\nsource: https://login.case.edu/\nsummary: >-\n  CWRU has no public developer authentication surface — no API key issuance, no third-party OAuth\n  client registration, no documented token endpoint for outside developers. What it does operate\n  is institutional identity for its own members, in three stacks. Two of them (Apereo CAS and the\n  Shibboleth IdP) run on CWRU's own registrable domain at login.case.edu; the third is a Microsoft\n  Entra ID tenant on Microsoft's host. All three answer unauthenticated metadata or protocol\n  requests, which is what makes them readable at all.\nmechanisms:\n  - id: shibboleth-idp\n\
  \    type: saml2-idp\n    operator: institution\n    entity_id: urn:mace:incommon:case.edu\n    metadata_url: https://mdq.incommon.org/entities/urn%3Amace%3Aincommon%3Acase.edu\n    sso_endpoints:\n      - https://login.case.edu/idp/profile/SAML2/Redirect/SSO\n      - https://login.case.edu/idp/profile/SAML2/POST/SSO\n      - https://login.case.edu/idp/profile/SAML2/POST-SimpleSign/SSO\n    scopes_asserted:\n      - case.edu\n      - artsci.case.edu\n      - dental.case.edu\n      - engineering.case.edu\n      - law.case.edu\n      - management.case.edu\n      - med.case.edu\n      - nursing.case.edu\n      - sass.case.edu\n    federation: InCommon (registrationAuthority https://incommon.org), exported to eduGAIN\n    audience: CWRU staff, students and federated service providers\n    public_client_registration: false\n    probed:\n      status: 200\n      content_type: application/samlmetadata+xml\n      bytes: 9543\n      valid_until: '2026-09-15T19:37:27.093Z'\n      date: '2026-09-01'\n\
  \    method: probed\n    source: https://mdq.incommon.org/entities/urn%3Amace%3Aincommon%3Acase.edu\n    note: >-\n      CWRU also self-hosts a metadata endpoint at https://login.case.edu/idp/shibboleth (200,\n      application/xml, 14,508 bytes) but it serves a NON-PRODUCTION descriptor — entityID\n      \"https://login-dev.case.edu/idp\", all bindings rebased onto login-dev.case.edu, with an XML\n      comment stating \"Still using old keypairs - fine for dev for now\". Consumers should take the\n      InCommon MDQ copy as authoritative. Recorded as an observed defect on CWRU's surface, not as\n      a second IdP.\n  - id: apereo-cas\n    type: cas-protocol\n    operator: institution\n    login_url: https://login.case.edu/cas/login\n    validate_endpoints:\n      - https://login.case.edu/cas/p3/serviceValidate\n    audience: CWRU applications integrating campus single sign-on\n    public_client_registration: false\n    probed:\n      url: https://login.case.edu/cas/p3/serviceValidate\n\
  \      status: 200\n      content_type: text/html;charset=UTF-8\n      body: >-\n        <cas:serviceResponse xmlns:cas='http://www.yale.edu/tp/cas'>\n        <cas:authenticationFailure code=\"INVALID_REQUEST\"></cas:authenticationFailure>\n        </cas:serviceResponse>\n      date: '2026-09-01'\n    method: probed\n    source: https://login.case.edu/cas/login\n    note: >-\n      An Apereo CAS deployment run by CWRU on its own domain. The CAS 3.0 protocol response\n      confirms the service is live and speaking the protocol; a valid ticket is required for any\n      real response, so this is an institution-operated authentication surface rather than a data\n      API. https://case.edu/ redirects to it, and https://canvas.case.edu/ redirects into\n      https://login.case.edu/idp/profile/SAML2/Redirect/SSO.\n  - id: entra-id-tenant\n    type: oidc-and-saml2\n    operator: federation\n    tenant_id: dc1c97ee-7a12-4624-9a01-9ad4f05d1311\n    issuer: https://login.microsoftonline.com/dc1c97ee-7a12-4624-9a01-9ad4f05d1311/v2.0\n\
  \    discovery_url: https://login.microsoftonline.com/case.edu/v2.0/.well-known/openid-configuration\n    saml_metadata_url: https://login.microsoftonline.com/dc1c97ee-7a12-4624-9a01-9ad4f05d1311/federationmetadata/2007-06/federationmetadata.xml\n    authorization_endpoint: https://login.microsoftonline.com/dc1c97ee-7a12-4624-9a01-9ad4f05d1311/oauth2/v2.0/authorize\n    token_endpoint: https://login.microsoftonline.com/dc1c97ee-7a12-4624-9a01-9ad4f05d1311/oauth2/v2.0/token\n    jwks_uri: https://login.microsoftonline.com/dc1c97ee-7a12-4624-9a01-9ad4f05d1311/discovery/v2.0/keys\n    audience: CWRU accounts on Microsoft 365 and Entra-integrated internal systems\n    public_client_registration: false\n    probed:\n      status: 200\n      bytes: 1964\n      tenant_region_scope: NA\n      date: '2026-09-01'\n    method: probed\n    source: https://login.microsoftonline.com/case.edu/v2.0/.well-known/openid-configuration\n    note: >-\n      login.microsoftonline.com is Microsoft's host and\
  \ Microsoft's contract. The TENANT is\n      CWRU's, resolved from the case.edu domain hint, which is why it is recorded as `federation`\n      rather than discarded as a vendor host.\nunauthenticated_surfaces:\n  - url: https://commons.case.edu/do/oai/?verb=Identify\n    detail: OAI-PMH harvesting of Scholarly Commons is open; no credential required.\n  - url: https://data.case.edu/api/3.19/serverinfo\n    detail: >-\n      Tableau Server REST serverInfo is unauthenticated by design and reports productVersion\n      2025.1.5, restApiVersion 3.25. Every other Tableau REST route requires a sign-in token.\n  - url: https://api.crossref.org/members/7530\n    detail: Crossref membership record; public.\n  - url: https://api.ror.org/v2/organizations/051fd9666\n    detail: ROR organization record; public.\ngated_surfaces:\n  - url: https://login.case.edu/cas/oidc/.well-known/openid-configuration\n    status: 401\n    detail: >-\n      The CAS OIDC module answers but refuses an unauthenticated\
  \ discovery read (401, 158 bytes).\n      Present but not publicly readable — recorded, not credited.\n  - url: https://login.case.edu/idp/status\n    status: 403\n    detail: Shibboleth IdP status page is IP-restricted; an access control, not a dead host.\n  - url: https://data.case.edu/\n    status: 200\n    detail: >-\n      Tableau Server SPA shell (vizportal, build 2025_1_34_2g69rzf1wzu). A 200 with no content —\n      every dashboard behind it requires CWRU sign-in.\nabsent_surfaces:\n  - url: https://api.case.edu/\n    status: 0\n    detail: Does not resolve.\n  - url: https://developer.case.edu/\n    status: 0\n    detail: Does not resolve.\n  - url: https://developers.case.edu/\n    status: 0\n    detail: Does not resolve.\n  - url: https://case.edu/llms.txt\n    status: 404\n    detail: No agent-facing site description.\n  - url: https://case.edu/.well-known/security.txt\n    status: 404\n    detail: No RFC 9116 security contact document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/case-western-reserve-university/refs/heads/main/authentication/case-western-reserve-university-authentication.yml
summary_line: 0 schemes
tags:
- Education
- Higher Education
- University
- Private Research University
- Association of American Universities
- Research
- Identity Federation
- Shibboleth
- SAML
- OAI-PMH
- Research Repository
- Library
- Course Catalog
- Crossref
- Cleveland
- Ohio
- United States
---
