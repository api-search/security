---
api_key_in: []
auth_types:
- none
- service-account
description: ''
kind: authentication
layout: security
method: searched
name: Casa Aviation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Civil Aviation Safety Authority (CASA) secures its APIs with none and service-account across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Civil Aviation Safety Authority (CASA)
provider_slug: casa-aviation
scheme_count: 2
schemes:
- applies_to:
  - casa-aviation:casa-airworthiness-directives-data
  - casa-aviation:casa-aircraft-register-data
  caveat: services.casa.gov.au returns HTTP 403 to unadorned programmatic clients (curl). This is an edge/bot filter, not an authentication requirement - the same URLs return 200 to a browser-like client.
  description: The Airworthiness Directives data files and the Australian Civil Aircraft Register data files are served without authentication. No API key, no account, no registration and no click-through terms acceptance were located on either data-files page.
  evidence: CASA's data-files pages publish direct download URLs with no credential instructions; combinedadweb.json was retrieved and parsed anonymously on 2026-07-28 (see review.yml probes).
  hosts:
  - https://services.casa.gov.au
  name: none
  type: none
- applies_to:
  - casa-aviation:casa-rpas-digital-platform
  credential_issuance:
    currently_open: partial
    environments:
    - name: staging
      note: Credentials issued once the initial written application is accepted and terms agreed.
    - name: development
      note: CASA internal only.
    - name: production
      note: Credentials issued only after the minimum requirements for approval are met.
    prerequisite: A paid Airservices Australia aeronautical/airspace data licence must be in place before CASA will consider approving access (Concept of Operations clause 13.1).
    process: Written application to CASA; acceptance of the RPAS Platform Terms and Conditions (four-year initial term); a Declaration of Compliance against the RPAS Platform Operating Rules; a live onboarding check-out against the RPAS Platform Test Procedure (two attempts permitted); and demonstrable compliance with Australian Government security and privacy requirements including the ASD Essential Eight, at the applicant's expense.
    self_serve: false
    status_note: New app providers may apply to onboard for Sydney Harbour AAA (R405A/R405B) and airspace awareness maps. CASA has paused onboarding of new providers for the ten trial aerodromes pending Airservices' Flight Information Management System (FIMS).
  description: The CASA RPAS Digital Platform feeds under data.casa.rpasplatform.net are accessed with a CASA-issued service account. The RPAS Platform Operating Rules (Attachment A) state for the notifications feed that the "URL needs authentication with a service account". No public token endpoint, no OAuth metadata and no self-serve credential issuance exists.
  evidence:
  - note: Attachment A names the endpoints and the service-account requirement.
    source: https://www.casa.gov.au/sites/default/files/2022-06/rpas-platform-operating-rules.pdf
  - note: Platform environments and minimum requirements for approval.
    source: https://www.casa.gov.au/sites/default/files/2021-09/rpas-platform-concept-of-operations.pdf
  - note: Agreement term, licence grant and termination conditions.
    source: https://www.casa.gov.au/sites/default/files/2021-09/rpas-platform-terms-conditions.pdf
  hosts:
  - https://data.casa.rpasplatform.net
  name: rpas-platform-service-account
  type: serviceAccount
slug: casa-aviation-authentication
source_filename: casa-aviation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource: >-\n  https://www.casa.gov.au/sites/default/files/2022-06/rpas-platform-operating-rules.pdf\ndocs:\n  - https://www.casa.gov.au/aircraft/aircraft-registration/data-files-registered-aircraft\n  - https://www.casa.gov.au/aircraft/airworthiness/airworthiness-directives/data-files-all-airworthiness-directives\n  - https://www.casa.gov.au/drones/industry-initiatives/digital-platform\nnote: >-\n  CASA publishes no OpenAPI, so no securityScheme could be derived mechanically.\n  This profile is read from CASA's own published documentation and the public\n  RPAS Platform reference PDFs. Two surfaces are anonymous; one is gated by a\n  CASA-issued service account.\nsummary:\n  types:\n    - none\n    - service-account\n  api_key_in: []\n  oauth2_flows: []\n  anonymous_surfaces: 2\n  gated_surfaces: 1\nschemes:\n  - name: none\n    type: none\n    applies_to:\n      - casa-aviation:casa-airworthiness-directives-data\n      - casa-aviation:casa-aircraft-register-data\n\
  \    description: >-\n      The Airworthiness Directives data files and the Australian Civil Aircraft\n      Register data files are served without authentication. No API key, no\n      account, no registration and no click-through terms acceptance were\n      located on either data-files page.\n    hosts:\n      - https://services.casa.gov.au\n    evidence: >-\n      CASA's data-files pages publish direct download URLs with no credential\n      instructions; combinedadweb.json was retrieved and parsed anonymously on\n      2026-07-28 (see review.yml probes).\n    caveat: >-\n      services.casa.gov.au returns HTTP 403 to unadorned programmatic clients\n      (curl). This is an edge/bot filter, not an authentication requirement -\n      the same URLs return 200 to a browser-like client.\n  - name: rpas-platform-service-account\n    type: serviceAccount\n    applies_to:\n      - casa-aviation:casa-rpas-digital-platform\n    description: >-\n      The CASA RPAS Digital Platform feeds under\
  \ data.casa.rpasplatform.net are\n      accessed with a CASA-issued service account. The RPAS Platform Operating\n      Rules (Attachment A) state for the notifications feed that the \"URL needs\n      authentication with a service account\". No public token endpoint, no\n      OAuth metadata and no self-serve credential issuance exists.\n    hosts:\n      - https://data.casa.rpasplatform.net\n    credential_issuance:\n      self_serve: false\n      process: >-\n        Written application to CASA; acceptance of the RPAS Platform Terms and\n        Conditions (four-year initial term); a Declaration of Compliance against\n        the RPAS Platform Operating Rules; a live onboarding check-out against\n        the RPAS Platform Test Procedure (two attempts permitted); and\n        demonstrable compliance with Australian Government security and privacy\n        requirements including the ASD Essential Eight, at the applicant's\n        expense.\n      environments:\n        - name: staging\n\
  \          note: Credentials issued once the initial written application is accepted and terms agreed.\n        - name: development\n          note: CASA internal only.\n        - name: production\n          note: Credentials issued only after the minimum requirements for approval are met.\n      prerequisite: >-\n        A paid Airservices Australia aeronautical/airspace data licence must be\n        in place before CASA will consider approving access (Concept of\n        Operations clause 13.1).\n      currently_open: partial\n      status_note: >-\n        New app providers may apply to onboard for Sydney Harbour AAA\n        (R405A/R405B) and airspace awareness maps. CASA has paused onboarding of\n        new providers for the ten trial aerodromes pending Airservices'\n        Flight Information Management System (FIMS).\n    evidence:\n      - source: https://www.casa.gov.au/sites/default/files/2022-06/rpas-platform-operating-rules.pdf\n        note: Attachment A names the endpoints\
  \ and the service-account requirement.\n      - source: https://www.casa.gov.au/sites/default/files/2021-09/rpas-platform-concept-of-operations.pdf\n        note: Platform environments and minimum requirements for approval.\n      - source: https://www.casa.gov.au/sites/default/files/2021-09/rpas-platform-terms-conditions.pdf\n        note: Agreement term, licence grant and termination conditions.\nnot_found:\n  - No OAuth 2.0 or OpenID Connect surface on casa.gov.au, services.casa.gov.au\n    or data.casa.rpasplatform.net.\n  - No API key issuance, developer account or key-management console.\n  - No /.well-known/openid-configuration or /.well-known/oauth-authorization-server.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/casa-aviation/refs/heads/main/authentication/casa-aviation-authentication.yml
summary_line: none/service-account · 2 schemes
tags:
- Travel
- Australia
- Aviation
- Airports
- Government
- Regulator
- Aviation Safety
- Open Data
- Drones
---
