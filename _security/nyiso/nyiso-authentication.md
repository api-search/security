---
api_key_in: []
auth_types:
- none
- http
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Nyiso Authentication
name_suffix: Authentication
oauth_flows: []
overview: New York Independent System Operator (NYISO) secures its APIs with none, http, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: New York Independent System Operator (NYISO)
provider_slug: nyiso
scheme_count: 3
schemes:
- description: HTTP Basic credential carrying a valid NYISO Market Information System (MIS) user account and its password. The account must hold the relevant metering or settlement privileges, granted by the participant's own Marketplace administrator per the NYISO Settlement Data Applications User's Guide.
  in: header
  name: MISBasicAuth
  parameter: Authorization
  scheme: basic
  sources:
  - https://www.nyiso.com/documents/20142/27889215/NYISO%20Metering%20API%20User%20Guide.pdf/d8ed36d3-1a40-9584-6961-3fdb845ca4fa
  - https://www.nyiso.com/documents/20142/45334160/NYISO%20Finance%20APIs%20User's%20Guide%20v1.2%20-%20DRAFT.pdf/4f0de58a-783d-a317-64fe-caed77ba61fa
  type: http
- description: A digital certificate issued by a NAESB-Authorized Certification Authority and bound to the MIS user account, presented on every request. This is the second factor - Basic credentials alone are not sufficient. Certificate acquisition and MIS account binding are described in the NYISO Market Participant User's Guide (MPUG).
  name: NAESBClientCertificate
  sources:
  - https://www.nyiso.com/documents/20142/3625950/mpug.pdf
  type: mutualTLS
- description: The MIS public archive and the OASIS postings bucket require no authentication of any kind.
  name: None
  type: none
slug: nyiso-authentication
source_filename: nyiso-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  NYISO Metering API User Guide (section 2.1-2.3) and NYISO Finance APIs User's\n  Guide v1.2 DRAFT (section 2.1-2.3), plus anonymous HTTP probes of every NYISO\n  host on 2026-07-27\ndocs: https://www.nyiso.com/manuals-tech-bulletins-user-guides\nsummary:\n  types:\n  - none\n  - http\n  - mutualTLS\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    NYISO runs two completely different authentication postures on two\n    completely different surfaces. The open data surfaces have no authentication\n    at all. The REST APIs use documented two-factor authentication - HTTP Basic\n    with an MIS user account plus a NAESB-accredited client certificate. There is\n    no API key, no OAuth 2.0, no OpenID Connect and no bearer token anywhere in\n    the NYISO estate, and no /.well-known/ discovery document exists to describe\n    one.\nsurfaces:\n- surface: MIS public data archive\n  base_url: http://mis.nyiso.com/public\n\
  \  scheme: none\n  description: >-\n    Fully anonymous HTTP/HTTPS GET. No account, no key, no application, no\n    referrer check and no licence click-through. Verified by anonymous probe on\n    2026-07-27 - daily CSV and monthly ZIP files returned 200 text/csv with no\n    credentials presented.\n  evidence: http://mis.nyiso.com/public/csv/rtfuelmix/20260726rtfuelmix.csv returned 200\n- surface: OASIS postings\n  base_url: https://oasis-postings.nyiso.com\n  scheme: none\n  description: >-\n    Anonymously readable object store. An unauthenticated ListBucket request\n    returned 200 application/xml and individual posting objects returned 200.\n  evidence: https://oasis-postings.nyiso.com/ACTIVE_TRANSMISSION_NODE/CSV/activetransmissionnodes.csv returned 200\n- surface: Finance APIs and Metering API\n  base_url: https://api.nyiso.com\n  scheme: two-factor - HTTP Basic plus NAESB client certificate\n  description: >-\n    Restricted to NYISO market participants. Both published user guides\
  \ state the\n    same requirement verbatim - \"A valid MIS user account and associated password\n    must be provided using Basic authentication\" and \"The NAESB certificate\n    associated with the MIS user account must be provided with each request\".\n    All endpoints answered 401 Authorization Required to anonymous probes.\n  evidence: https://api.nyiso.com/finance/metering/v1/powerMetering returned 401\nschemes:\n- name: MISBasicAuth\n  type: http\n  scheme: basic\n  in: header\n  parameter: Authorization\n  description: >-\n    HTTP Basic credential carrying a valid NYISO Market Information System (MIS)\n    user account and its password. The account must hold the relevant metering or\n    settlement privileges, granted by the participant's own Marketplace\n    administrator per the NYISO Settlement Data Applications User's Guide.\n  sources:\n  - https://www.nyiso.com/documents/20142/27889215/NYISO%20Metering%20API%20User%20Guide.pdf/d8ed36d3-1a40-9584-6961-3fdb845ca4fa\n  - https://www.nyiso.com/documents/20142/45334160/NYISO%20Finance%20APIs%20User's%20Guide%20v1.2%20-%20DRAFT.pdf/4f0de58a-783d-a317-64fe-caed77ba61fa\n\
  - name: NAESBClientCertificate\n  type: mutualTLS\n  description: >-\n    A digital certificate issued by a NAESB-Authorized Certification Authority\n    and bound to the MIS user account, presented on every request. This is the\n    second factor - Basic credentials alone are not sufficient. Certificate\n    acquisition and MIS account binding are described in the NYISO Market\n    Participant User's Guide (MPUG).\n  sources:\n  - https://www.nyiso.com/documents/20142/3625950/mpug.pdf\n- name: None\n  type: none\n  description: >-\n    The MIS public archive and the OASIS postings bucket require no\n    authentication of any kind.\ntransport:\n  documented: HTTPS 1.1 over TLS 1.2\n  observed: >-\n    api.nyiso.com and apitest.nyiso.com negotiate both TLS 1.2 and TLS 1.3 as of\n    the 2026-07-27 probe; the guides state TLS 1.2 as the documented minimum.\n  note: >-\n    mis.nyiso.com also serves the public archive over plain HTTP, which is how\n    NYISO's own list pages link it.\nonboarding:\n\
  \  self_serve: false\n  path: >-\n    Become a registered NYISO Market Participant, obtain an MIS user account with\n    metering/settlement privileges through your organization's Marketplace\n    administrator, then obtain a NAESB-accredited digital certificate bound to\n    that account. There is no developer sign-up form and no anonymous trial - the\n    market-trial host apitest.nyiso.com is credentialed too.\n  contact: Stakeholder_Services@nyiso.com / +1 518-356-6060\n  guides:\n  - https://www.nyiso.com/documents/20142/3625950/mpug.pdf\n  - https://www.nyiso.com/documents/20142/3625950/SDA_UG.pdf\ndiscovery:\n  well_known_openid_configuration: 404\n  well_known_oauth_authorization_server: 404\n  note: See well-known/nyiso-well-known.yml for the full probe record.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nyiso/refs/heads/main/authentication/nyiso-authentication.yml
summary_line: none/http/mutualTLS · 3 schemes
tags:
- Energy
- United States
- Electricity
- Energy Markets
- Grid
- Open Data
- System Operator
- New York
- Renewables
- Emissions
---
