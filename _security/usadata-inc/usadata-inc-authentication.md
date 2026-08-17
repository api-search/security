---
api_key_in: []
auth_types:
- custom-soap-body-credential
description: USADATA Leads Engine authenticates with a credential triple carried in the SOAP request BODY, not in a transport header. Every operation except the two unauthenticated diagnostics (ping, getVersion) declares a leading `Login` element of type `{http://Usadata.com/Services/LeadsEngine/Login}Login`. There is no WS-Security header, no OAuth, no API-key header and no bearer token in the published contract; credentials are issued by USADATA through its sales / developer-support process (there is no self-service API sign-up).
kind: authentication
layout: security
method: derived
name: Usadata Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: USADATA, Inc. secures its APIs with custom-soap-body-credential across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: USADATA, Inc.
provider_slug: usadata-inc
scheme_count: 1
schemes:
- applies_to_operations: 22
  element: Login
  fields:
  - name: UserID
    note: minOccurs="0" in the schema; supplied in practice.
    required: false
    type: string
  - name: Password
    note: Cleartext password element in the request body. There is no digest, nonce, timestamp or signature in the contract, so confidentiality rests entirely on TLS.
    required: false
    type: string
  - name: ClientID
    note: Tenant / account identifier alongside the user credential.
    required: false
    type: string
  location: soap-body
  name: Login
  namespace: http://Usadata.com/Services/LeadsEngine/Login
  sources:
  - wsdl/usadata-inc-leads-engine.wsdl
  type: custom
slug: usadata-inc-authentication
source_filename: usadata-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: wsdl/usadata-inc-leads-engine.wsdl\ndescription: >-\n  USADATA Leads Engine authenticates with a credential triple carried in the\n  SOAP request BODY, not in a transport header. Every operation except the two\n  unauthenticated diagnostics (ping, getVersion) declares a leading `Login`\n  element of type `{http://Usadata.com/Services/LeadsEngine/Login}Login`. There\n  is no WS-Security header, no OAuth, no API-key header and no bearer token in\n  the published contract; credentials are issued by USADATA through its sales /\n  developer-support process (there is no self-service API sign-up).\nsummary:\n  types:\n  - custom-soap-body-credential\n  api_key_in: []\n  oauth2_flows: []\n  transport: https\n  soap_bindings:\n  - SOAP 1.1\n  - SOAP 1.2\nschemes:\n- name: Login\n  type: custom\n  location: soap-body\n  element: Login\n  namespace: http://Usadata.com/Services/LeadsEngine/Login\n  sources:\n  - wsdl/usadata-inc-leads-engine.wsdl\n\
  \  fields:\n  - name: UserID\n    type: string\n    required: false\n    note: minOccurs=\"0\" in the schema; supplied in practice.\n  - name: Password\n    type: string\n    required: false\n    note: >-\n      Cleartext password element in the request body. There is no digest,\n      nonce, timestamp or signature in the contract, so confidentiality rests\n      entirely on TLS.\n  - name: ClientID\n    type: string\n    required: false\n    note: Tenant / account identifier alongside the user credential.\n  applies_to_operations: 22\nanonymous_operations:\n- operation: ping\n  evidence: >-\n    Live SOAP 1.1 POST to https://leadsengine.usadata.com/service.asmx with\n    SOAPAction \"http://Usadata/Services/Service/ping\" and no Login element\n    returned HTTP 200 with <pingResult>true</pingResult> on 2026-08-13.\n- operation: getVersion\n  evidence: >-\n    Live SOAP 1.1 POST with SOAPAction\n    \"http://Usadata/Services/Service/getVersion\" and no Login element returned\n    HTTP\
  \ 200 with <getVersionResult>3.0.9719.28036</getVersionResult> on\n    2026-08-13.\npartial_credential_operations:\n- operation: getAvailablePriorOrders\n  note: >-\n    Does NOT take the Login element. It takes AppID + AccountID + DataSource +\n    Interval as plain string parameters, which is a different (and weaker)\n    credential shape than every sibling operation. Recorded as observed, not\n    endorsed.\nnotes:\n- No self-service credential issuance was found. www.usadata.com/products/apis\n  advertises \"RESTful API, full documentation, sandbox, dedicated developer\n  support\" but routes to \"Request A Demo\" / \"Talk To A Developer\"; no developer\n  portal, key-management console or auth reference page is published.\n- The published Leads Engine contract is SOAP/WSDL, not the REST API the\n  marketing page describes. No REST contract was found on any USADATA host\n  (see well-known/usadata-inc-well-known.yml for the probe record).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usadata-inc/refs/heads/main/authentication/usadata-inc-authentication.yml
summary_line: custom-soap-body-credential · 1 scheme
tags:
- Company
- Data
- Marketing
- Data Enrichment
- Audience Targeting
- Data Hygiene
- Direct Mail
- Leads
- SOAP
- Mailing Lists
---
