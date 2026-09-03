---
api_key_in: []
api_specs:
- filename: king-saud-university-open-data-openapi.yml
  format: yaml
  label: KSU Open Data Distribution API
  slug: open-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/king-saud-university/refs/heads/main/openapi/king-saud-university-open-data-openapi.yml
- filename: king-saud-university-identity-openapi.yml
  format: yaml
  label: KSU Identity and Access Management (OAuth 2.0 / OpenID Connect / SAML 2.0)
  slug: identity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/king-saud-university/refs/heads/main/openapi/king-saud-university-identity-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: King Saud University Authentication
name_suffix: Authentication
oauth_flows: []
overview: King Saud University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: King Saud University
provider_slug: king-saud-university
scheme_count: 0
schemes: []
slug: king-saud-university-authentication
source_filename: king-saud-university-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live anonymous HTTP probes of https://data.ksu.edu.sa on 2026-09-01, plus the\n  SAML AuthnRequest issued by https://lms.ksu.edu.sa and the King Saud University\n  entity record in the eduGAIN interfederation metadata.\nx-operator: institution\nsummary: >-\n  King Saud University runs two entirely separate authentication postures. Its\n  open-data distribution surface is fully anonymous — no key, no token, no\n  registration. Everything else the university exposes is behind a single\n  institutional SAML 2.0 identity provider, and there is no OAuth/OIDC developer\n  authorization path of any kind.\nsurfaces:\n  - surface: Open Data distributions\n    host: data.ksu.edu.sa\n    x-operator: institution\n    scheme: none\n    anonymous: true\n    registration_required: false\n    detail: >-\n      All 852 dataset distribution files were served to an unauthenticated client\n      with no cookie, key or referer. 20 of 20 sampled\
  \ files returned HTTP 200.\n      The open-data licence at https://data.ksu.edu.sa/ar/node/1178 grants use\n      \"to all persons without discrimination or charge\" and asks only for source\n      attribution.\n    evidence:\n      - url: https://data.ksu.edu.sa/sites/data.ksu.edu.sa/files/users/user976/KSU-DMO-OD-DATASET-Employees-1444-AH.json\n        status: 200\n      - url: https://data.ksu.edu.sa/ar/node/1178\n        status: 200\n  - surface: Institutional single sign-on (SAML 2.0 identity provider)\n    host: iam.ksu.edu.sa\n    x-operator: institution\n    scheme: saml2\n    protocol_binding: HTTP-POST / HTTP-Redirect SP-initiated SSO\n    idp_entity_id: http://SSO.ksu.edu.sa/adfs/services/trust\n    idp_sso_endpoint: https://iam.ksu.edu.sa/idp/startSSO.ping\n    software: PingFederate (the eduGAIN-registered entityID still carries the\n      university's earlier ADFS identifier)\n    scope: ksu.edu.sa\n    registration_authority: https://www.maeen.sa\n    federation: Maeen Identity\
  \ Federation (SA-MIF), a member of eduGAIN since\n      2019-07-02; the King Saud University IdP entity has been in eduGAIN since\n      2020-02-02.\n    detail: >-\n      Requesting https://lms.ksu.edu.sa/ returns a self-submitting SAML\n      AuthnRequest form whose action is\n      https://iam.ksu.edu.sa/idp/startSSO.ping?PartnerSpId=https%3A%2F%2Flms.ksu.edu.sa\n      — direct evidence that KSU operates the IdP itself rather than delegating\n      identity to a vendor. The IdP's own SAML metadata is not served anonymously\n      (/idp/shibboleth and /idp/metadata both 404); it is distributed through the\n      Maeen federation into the eduGAIN aggregate.\n    evidence:\n      - url: https://lms.ksu.edu.sa/\n        status: 200\n      - url: https://iam.ksu.edu.sa/\n        status: 200\n      - url: https://mds.edugain.org/edugain-v2.xml\n        status: 200\n      - url: https://technical.edugain.org/entities?id=671188\n        status: 200\n      - url: https://iam.ksu.edu.sa/idp/shibboleth\n\
  \        status: 404\n  - surface: Gated end-user applications\n    hosts:\n      - edugate.ksu.edu.sa\n      - my.ksu.edu.sa\n      - e.ksu.edu.sa\n      - faculty.ksu.edu.sa\n    x-operator: institution\n    scheme: institutional-login\n    detail: >-\n      The Edugate student information system, the MyKSU portal, the KSUEgate\n      single-sign-on gateway and the faculty portal are end-user web applications\n      behind institutional credentials. No public API reference, token endpoint or\n      developer registration exists for any of them.\nabsent:\n  - scheme: oauth2\n    reason: No authorization server, client registration or token endpoint published.\n  - scheme: apiKey\n    reason: No key issuance path; the open-data surface needs none.\n  - scheme: openIdConnect\n    reason: >-\n      No .well-known/openid-configuration served on ksu.edu.sa, iam.ksu.edu.sa or\n      data.ksu.edu.sa.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/king-saud-university/refs/heads/main/authentication/king-saud-university-authentication.yml
summary_line: 0 schemes
tags:
- Education
- Higher Education
- University
- Public Research University
- Saudi Arabia
- Middle East
- Riyadh
- Open Data
- Research Data
- Identity Federation
- Single Sign-On
- Research
- Linked Data
---
