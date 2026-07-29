---
api_key_in:
- header
auth_types:
- apiKey
description: 'Air Canada''s NDC API is authenticated by a single opaque API key issued by Air Canada, carried in an "apikey" HTTP header on every SOAP request, plus an in-payload identity chain that the platform authorises against: the SellerID in the aggregation envelope and, for agency flows, the accredited IATA number and Agency ID inside the IATA NDC message itself. There is no OAuth, no OpenID Connect and no self-service key issuance on the inbound path - keys are handed out only after a commercial agreement and certification. OAuth appears in exactly one place, and it is outbound: when a seller registers a webhook to receive OrderChangeNotification messages, Air Canada supports OAuth as the authentication method it will use when calling the seller''s endpoint.'
kind: authentication
layout: security
method: searched
name: Air Canada Authentication
name_suffix: Authentication
oauth_flows: []
overview: Air Canada secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Air Canada
provider_slug: air-canada
scheme_count: 2
schemes:
- description: '"The API key is a unique authorization key issued by Air Canada. To access the Air Canada NDC Platform API, each seller should provide the ''apikey'' in the HTTP header." (verbatim, API Setup page)'
  environments:
  - base_url: https://gold-ndcpartners.aircanada.com/
    name: gold (sandbox / certification)
  - base_url: https://ndcpartners.aircanada.com/
    name: production
  failure_mode: '"Please be sure to add this or you will experience an authentication error (i.e., 400 Bad Request)." (verbatim)'
  in: header
  name: apikey
  parameter_name: apikey
  sources:
  - https://ndc.aircanada.com/api/gettingstarted/apisetup
  type: apiKey
- description: 'Formerly required alongside apikey on OrderCreateRQ and OrderChangeRQ. Air Canada now states verbatim: "NOTE: You no longer need to submit the two additional parameters given below, when sending an OrderCreateRQ or OrderChangeRQ" (TP-Proxy-Key and Tx-http-timeout).'
  in: header
  name: TP-Proxy-Key
  parameter_name: TP-Proxy-Key
  sources:
  - https://ndc.aircanada.com/api/gettingstarted/apisetup
  status: retired
  type: apiKey
slug: air-canada-authentication
source_filename: air-canada-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource: https://ndc.aircanada.com/api/gettingstarted/apisetup\ndocs: https://ndc.aircanada.com/api/gettingstarted/apisetup\ndescription: >-\n  Air Canada's NDC API is authenticated by a single opaque API key issued by Air\n  Canada, carried in an \"apikey\" HTTP header on every SOAP request, plus an\n  in-payload identity chain that the platform authorises against: the SellerID\n  in the aggregation envelope and, for agency flows, the accredited IATA number\n  and Agency ID inside the IATA NDC message itself. There is no OAuth, no\n  OpenID Connect and no self-service key issuance on the inbound path - keys are\n  handed out only after a commercial agreement and certification. OAuth appears\n  in exactly one place, and it is outbound: when a seller registers a webhook to\n  receive OrderChangeNotification messages, Air Canada supports OAuth as the\n  authentication method it will use when calling the seller's endpoint.\nsummary:\n\
  \  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  self_service_issuance: false\n  gate: commercial agreement + display certification + accredited IATA/ARC codes\nschemes:\n  - name: apikey\n    type: apiKey\n    in: header\n    parameter_name: apikey\n    description: >-\n      \"The API key is a unique authorization key issued by Air Canada. To access\n      the Air Canada NDC Platform API, each seller should provide the 'apikey' in\n      the HTTP header.\" (verbatim, API Setup page)\n    failure_mode: >-\n      \"Please be sure to add this or you will experience an authentication error\n      (i.e., 400 Bad Request).\" (verbatim)\n    environments:\n      - name: gold (sandbox / certification)\n        base_url: https://gold-ndcpartners.aircanada.com/\n      - name: production\n        base_url: https://ndcpartners.aircanada.com/\n    sources: [https://ndc.aircanada.com/api/gettingstarted/apisetup]\n  - name: TP-Proxy-Key\n    type: apiKey\n    in: header\n    parameter_name:\
  \ TP-Proxy-Key\n    status: retired\n    description: >-\n      Formerly required alongside apikey on OrderCreateRQ and OrderChangeRQ. Air\n      Canada now states verbatim: \"NOTE: You no longer need to submit the two\n      additional parameters given below, when sending an OrderCreateRQ or\n      OrderChangeRQ\" (TP-Proxy-Key and Tx-http-timeout).\n    sources: [https://ndc.aircanada.com/api/gettingstarted/apisetup]\nin_payload_identity:\n  description: >-\n    Authorisation is not carried by the API key alone. The NDC aggregation\n    envelope and the IATA message both carry identity elements that Air Canada\n    validates, and error code 89975 (\"The validation of OfficeID and credentials\n    has resulted in failure\") is returned when they do not line up.\n  elements:\n    - element: NDCMSG_Header/Sender/SellerID\n      required: true\n      description: The seller's key in the aggregation (SOAP) envelope. Example value in the docs is ac.gndc.Test.\n    - element: NDCMSG_Header/Recipient/Address/Company\n\
  \      required: true\n      description: Offer owner airline designator; AC for Air Canada.\n    - element: Party/Sender/TravelAgencySender/IATA_Number\n      required: for agency bookings\n      description: >-\n        The seller's accredited 8-digit IATA number (or TIDS). Air Canada\n        documents \"In production, sellers must pass their accredited IATA codes\n        only\" and \"Do not use any IATA codes that are used in examples.\"\n    - element: Party/Sender/TravelAgencySender/AgencyID\n      required: true\n      description: Agency identifier provided by Air Canada. Example value in the docs is 493.\n    - element: Party/Sender/TravelAgencySender/PseudoCity\n      required: false\n    - element: Party/Sender/TravelAgencySender/AgentUser/AgentUserID\n      required: false\n    - element: PointOfSale/Location/CountryCode\n      required: mandatory for direct consumer flows, optional for agency bookings\noutbound_callback_auth:\n  surface: OrderChangeNotification (OCN) webhook\n\
  \  description: >-\n    Sellers registering to receive OCN messages must supply, verbatim: \"Webhook\n    host, Webhook URL, Authentication method (OAuth), AT system credentials, PRD\n    system credentials, OAuthTokenURL (if OAuth is the authentication method),\n    OAuthScope (if OAuth is the authentication method), Any headers required in\n    the request.\"\n  registration_contact: ACDirectconnectNDC@aircanada.ca\n  detail: asyncapi/air-canada-ocn-webhooks.yml\nauthentication_errors_detail: errors/air-canada-error-codes.yml\nauthentication_errors:\n  - code: 89975\n    message: The validation of OfficeID and credentials has resulted in failure and hence, cannot proceed with the shopping search\n  - code: 199994\n    message: CompanyShortName is not supported\n  - code: 199999\n    message: IATA not allowed\n  - code: 1533\n    message: INVALID OFFICE IDENTIFICATION CODE\n  - code: 1914\n    message: OFFICE RESTRICTED\nnot_supported:\n  - oauth2 (inbound)\n  - openIdConnect\n  - mutualTLS\
  \ (not documented)\n  - http basic / bearer\n  - self-service key generation or rotation portal\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/air-canada/refs/heads/main/authentication/air-canada-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Travel
- Canada
- Aviation
- Airline
- NDC
- Distribution
- Booking
- Airlines
- Loyalty
---
