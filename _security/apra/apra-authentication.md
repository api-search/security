---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Apra Authentication
name_suffix: Authentication
oauth_flows: []
overview: APRA declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: APRA
provider_slug: apra
scheme_count: 0
schemes: []
slug: apra-authentication
source_filename: apra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://www.apra.gov.au/apra-portals/apra-connect/apra-connect-information-security-and-technical-specifications\ndocs:\n- https://www.apra.gov.au/apra-portals/apra-connect/accessing-apra-connect\n- https://www.apra.gov.au/apra-portals/apra-connect/apra-connect-information-security-and-technical-specifications\nsummary:\n  types: []\n  api_auth: none\n  note: >-\n    There are no OpenAPI securitySchemes to derive from because APRA publishes no API.\n    APRA's own technical specifications page lists the \"API technical specification\"\n    as \"to be provided when this functionality is available\". The authentication model\n    below is the documented, human, browser-based authentication for APRA Connect —\n    the only integration surface APRA operates — and is recorded so the auth posture\n    is legible, not to imply an API auth scheme exists.\napi_authentication:\n  api_key: false\n  http_basic: false\n  http_bearer: false\n\
  \  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  evidence:\n  - https://www.apra.gov.au/.well-known/openid-configuration returned 404\n  - https://www.apra.gov.au/.well-known/oauth-authorization-server returned 404\n  - connect.apra.gov.au /.well-known/* return F5 WAF \"Request Rejected\" HTML, not\n    discovery metadata (see well-known/apra-well-known.yml)\nportal_authentication:\n  model: federated human SSO via the Australian Government Digital ID System\n  identity_provider:\n    name: myID\n    role: identity provider (Digital ID)\n    strength_required: Standard\n    url: https://www.ato.gov.au/General/Online-services/Accessing-online-services-with-myGovID-and-RAM/\n  authorisation:\n    name: Relationship Authorisation Manager (RAM)\n    role: links a Digital ID to the organisation (by ABN) it acts for\n    url: https://info.authorisationmanager.gov.au/\n  digital_id_system: https://www.digitalidsystem.gov.au/what-is-digital-id\n  flow:\n  - Each user obtains their\
  \ own Digital ID (myID) at Standard strength\n  - A principal authority links the organisation in RAM; authorised users and\n    administrators are then authorised against that organisation's ABN\n  - The entity nominates one Regulatory Reporting Administrator (RRA) per ABN via the\n    APRA Connect RRA nomination form; APRA administrators assign the initial RRA role\n  - The RRA assigns roles and permissions to all other users of that entity\n  - \"At login: go to connect.apra.gov.au, choose Continue with Digital ID, select myID,\n    enter the myID email, confirm the four-digit code in the myID app, and consent to\n    the attribute release\"\n  service_providers: >-\n    Third-party service providers submitting on an entity's behalf must be authorised\n    in RAM by that entity's principal authority or authorisation administrator —\n    against the entity's ABN, not their own.\n  environments:\n    production: https://connect.apra.gov.au\n    test: https://connect-test.apra.gov.au\n\
  \    note: Production and test are separate; there is no data transfer between them and\n      users must be enrolled in each environment independently.\nauthorisation_model:\n  scheme: entity-scoped roles managed by the entity\n  roles:\n  - name: Regulatory Reporting Administrator (RRA)\n    note: The only role that can manage user access for an entity. One nominated per ABN.\n  - name: Corporate Profile User\n    note: Assigned to the initial RRA in the test environment alongside ad hoc return\n      permissions.\n  note: >-\n    APRA publishes no scope or permission reference (there is no OAuth surface), so\n    scopes/ is intentionally absent for this provider.\naccess_monitoring:\n  quarterly_download_extract: >-\n    APRA sends each entity a quarterly email extract of APRA Connect file downloads —\n    dates, times and source IP addresses — so entities can validate that only\n    authorised systems accessed their data, with a follow-up process for usernames and\n    file names.\n\
  \  source: https://www.apra.gov.au/apra-portals/apra-connect/apra-connect-support-material\nschemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apra/refs/heads/main/authentication/apra-authentication.yml
summary_line: 0 schemes
tags:
- Insurance
- Australia
- Regulator
- Prudential Regulation
- General Insurance
- Life Insurance
- Private Health Insurance
- Regulatory Reporting
- Market Infrastructure
- Risk Data
- Superannuation
- Banking
---
