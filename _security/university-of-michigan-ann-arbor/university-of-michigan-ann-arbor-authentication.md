---
api_key_in: []
api_specs:
- filename: university-of-michigan-ann-arbor-deep-blue-documents-oai-pmh-openapi.yml
  format: yaml
  label: Deep Blue Documents OAI-PMH
  slug: deep-blue-documents-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-michigan-ann-arbor/refs/heads/main/openapi/university-of-michigan-ann-arbor-deep-blue-documents-oai-pmh-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: University Of Michigan Ann Arbor Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Michigan-Ann Arbor declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Michigan-Ann Arbor
provider_slug: university-of-michigan-ann-arbor
scheme_count: 0
schemes: []
slug: university-of-michigan-ann-arbor-authentication
source_filename: university-of-michigan-ann-arbor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nname: University of Michigan-Ann Arbor — Authentication\ngenerated: '2026-08-19'\nmethod: probed\nsource: >-\n  Live probes 2026-08-19 of shibboleth.umich.edu, weblogin.umich.edu, mdq.incommon.org,\n  backend.production.deepblue-documents.lib.umich.edu and mbus.ltp.umich.edu, plus the\n  published ITS API Directory getting-started documentation.\nnote: >-\n  U-M's authentication story is two entirely separate things, and conflating them is the easy\n  mistake. The institution operates a full federated identity provider — that is real,\n  machine-readable, institution-run infrastructure. It does NOT operate a public developer\n  authentication surface: the enterprise API estate is closed to anyone without a U-M account.\nsurfaces:\n  - surface: Deep Blue Documents OAI-PMH\n    operator: institution\n    scheme: none\n    description: >-\n      Unauthenticated and open. No API key, no bearer token, no registration. All six OAI-PMH\n      verbs answered anonymously with HTTP\
  \ 200 on 2026-08-19.\n    evidence: 'GET .../server/oai/request?verb=Identify -> 200 text/xml, no credential supplied'\n  - surface: U-M ITS API Directory (Apigee X)\n    operator: institution\n    scheme: sso-gated\n    description: >-\n      Sign-in with a U-M uniqname and password, Duo two-factor authentication, and presence on\n      the U-M network or VPN are all required to browse, subscribe to, or consume any API in\n      the directory. Consumers then hold an API key/secret pair and exchange it for a token —\n      the shape is visible in U-M Library's own open-source client\n      (github.com/mlibrary/class_api_requester), which is constructed with an API id, an API\n      secret, an API URL and a separate token URL to call the Schedule of Classes API.\n    evidence: >-\n      https://its.umich.edu/data/data-database/api-directory/getting-started -> 403 to\n      automated agents (Cloudflare managed challenge, body \"Just a moment...\"); documented\n      access model corroborated\
  \ by ITS documentation and by mlibrary/class_api_requester.\n    public_credential_issuance: false\n  - surface: Magic Bus (mbus.ltp.umich.edu) BusTime API\n    operator: institution\n    scheme: api-key\n    description: >-\n      Query-string API access key. No public self-service key issuance page was found.\n    evidence: >-\n      GET https://mbus.ltp.umich.edu/bustime/api/v3/getroutes -> 200 text/xml,\n      '<bustime-response><error><msg>No API access key supplied</msg></error></bustime-response>'\nidentity_federation:\n  operator: institution\n  standard: SAML 2.0 / Shibboleth\n  entity_id: https://shibboleth.umich.edu/idp/shibboleth\n  metadata_url: https://shibboleth.umich.edu/idp/shibboleth\n  metadata_mirror: https://weblogin.umich.edu/idp/shibboleth\n  local_copy: authentication/university-of-michigan-ann-arbor-shibboleth-idp-metadata.xml\n  federation: InCommon\n  federation_registration_authority: https://incommon.org\n  federation_mdq: https://mdq.incommon.org/entities/https%3A%2F%2Fshibboleth.umich.edu%2Fidp%2Fshibboleth\n\
  \  scopes:\n    - umich.edu\n    - annarbor.umich.edu\n    - umd.umich.edu\n    - dearborn.umich.edu\n    - flint.umich.edu\n  display_name: University of Michigan\n  privacy_statement: https://it.umich.edu/security-privacy\n  entity_category: https://github.com/umich-iam/shibboleth-umich-federation/raw/master/category/prod.md\n  evidence: >-\n    GET https://shibboleth.umich.edu/idp/shibboleth -> 200 application/xml, 10,923 bytes;\n    GET https://mdq.incommon.org/entities/... -> 200 application/samlmetadata+xml, 9,252 bytes\n    with mdrpi:RegistrationInfo registrationAuthority=\"https://incommon.org\".\n  note: >-\n    U-M ITS Identity and Access Management publishes working SAML and OIDC service-provider\n    integration examples publicly at github.com/umich-iam (SSO-Examples plus fifteen\n    per-framework example repositories, and iam-api-examples). That is genuine, institution-authored\n    developer material — it just documents how to federate WITH U-M, not how to consume a U-M\
  \ API\n    without a U-M account.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-michigan-ann-arbor/refs/heads/main/authentication/university-of-michigan-ann-arbor-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Public Research University
- United States
- Michigan
- Big Ten
- Association of American Universities
- Research Data
- Institutional Repository
- Identity Federation
- OAI-PMH
- Library
- Research Computing
---
