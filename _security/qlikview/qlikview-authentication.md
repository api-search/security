---
api_key_in: []
auth_types: []
description: Authentication profile for the QlikView API surface, read from Qlik's own developer help rather than derived from a spec - QlikView publishes no OpenAPI, and its QMS contract is a WSDL served only from the customer's own installed server. There is NO OAuth 2.0, NO OpenID Connect and NO API-key surface anywhere in QlikView. Every documented mechanism is either Windows/NTFS identity on the customer's own network or a server-issued short-lived ticket, which is what an on-premises product of this generation looks like.
kind: authentication
layout: security
method: searched
name: Qlikview Authentication
name_suffix: Authentication
oauth_flows: []
overview: QlikView declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: QlikView
provider_slug: qlikview
scheme_count: 5
schemes:
- applies_to:
  - QlikView Management API (QMS API)
  - QlikView Server API
  - QlikView Distribution Service API (IQDS)
  description: Every QMS API operation must carry a service key in the X-Service-Key HTTP/HTTPS header. The single exception is GetTimeLimitedServiceKey, which is the operation used to OBTAIN a key and therefore cannot require one. Qlik states the header exists to prevent cross-site request forgery.
  id: qms-service-key
  in: header
  lifetime: Time-limited. The key is issued by GetTimeLimitedServiceKey and expires; clients must re-request rather than persist one.
  name: X-Service-Key
  obtain_operation: GetTimeLimitedServiceKey
  source: https://help.qlik.com/en-US/qlikview-developer/September2025/Subsystems/QMSAPIref/Content/Home.htm
  transport: SOAP over HTTP or HTTPS
  type: apiKey
- applies_to:
  - QlikView Management API (QMS API)
  - QlikView Distribution Service API (IQDS)
  description: Authorization for the QMS API is Windows local-group membership on the QlikView server, not scopes. Most operations require membership of the local group "QlikView Management API", which gates overall API access; individual operations additionally require "QlikView Administrator" or "QlikView EDX".
  groups:
  - grants: Overall QMS API access; required by most operations.
    name: QlikView Management API
  - grants: Administrative operations.
    name: QlikView Administrator
  - grants: External Document Exchange (EDX) task-trigger operations.
    name: QlikView EDX
  id: windows-group-authorization
  source: https://help.qlik.com/en-US/qlikview-developer/September2025/Subsystems/QMSAPIref/Content/Home.htm
  type: platform
- applies_to:
  - QlikView Authentication API (Ticket API)
  - QlikView AccessPoint API
  - QlikView Workbench API
  authorization_modes:
  - DMS - Document Metadata Service authorization by group name
  - NTFS - Windows authorization by Security Identifier (SID)
  description: Custom Ticket Exchange (CTE). A trusted third-party system POSTs a ticket request on behalf of an already-authenticated user; QlikView Server returns a ticket - "a string of random bytes" - which the browser then exchanges for a session. This is QlikView's single sign-on path for embedding and for portals that do the authentication themselves.
  endpoints:
  - method: POST
    path: /QvAJAXZfc/GetWebTicket.aspx
    purpose: Request a ticket for a named user.
    request_body_shape: <Global method="GetWebTicket"><UserId>[User Name]</UserId>[Groups]</Global>
    request_content_type: application/xml
    response_body_shape: <Global><_retval_>[Ticket]</_retval_></Global>
  - method: GET
    path: /QvAJAXZfc/Authenticate.aspx
    purpose: Redirect target that exchanges the ticket for a QlikView session.
  - method: POST
    path: /Accesspoint.aspx
    purpose: Terminate the session (logout).
  fields:
  - description: The user name the ticket is being minted for.
    name: UserId
    required: true
  - description: Optional list of group names, each wrapped in a <string> element.
    name: GroupList
    required: false
  - description: true when GroupList carries Document Metadata Service (DMS) group NAMES; false when it carries Windows Security Identifiers (SIDs) for NTFS authorization.
    name: GroupsIsNames
    required: false
  - description: The returned random-byte ticket, exchanged at Authenticate.aspx.
    name: Ticket
  id: custom-ticket-exchange
  source: https://help.qlik.com/en-US/qlikview-developer/September2025/Content/QV_HelpSites/Ticket-API.htm
  type: ticket
- applies_to:
  - QlikView AccessPoint API
  - QlikView Server API
  description: The default AccessPoint path is Windows integrated authentication (NTLM/Kerberos) against the domain the QlikView Server is joined to, with NTFS or DMS authorization on the documents themselves. No token is exchanged over the API; identity comes from the operating system.
  id: windows-integrated
  source: https://community.qlik.com/t5/Official-Support-Articles/Customized-Authentication-in-QlikView/ta-p/1710763
  type: platform
- applies_to:
  - QlikView Plugin API
  - QlikView OCX API (Automation API)
  - QlikView QVX SDK API
  description: In-process COM/.NET surfaces on the user's own desktop or server. There is no network authentication because there is no network call - the caller already runs as the Windows user.
  id: local-com
  type: none
slug: qlikview-authentication
source_filename: qlikview-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: >-\n  https://help.qlik.com/en-US/qlikview-developer/September2025/Subsystems/QMSAPIref/Content/Home.htm\n  and https://help.qlik.com/en-US/qlikview-developer/September2025/Content/QV_HelpSites/Ticket-API.htm\ndocs: https://help.qlik.com/en-US/qlikview-developer/September2025/Content/QV_HelpSites/APIsAndSDKs.htm\nprovider: QlikView\nproviderId: qlikview\ndescription: >-\n  Authentication profile for the QlikView API surface, read from Qlik's own developer help\n  rather than derived from a spec - QlikView publishes no OpenAPI, and its QMS contract is a\n  WSDL served only from the customer's own installed server. There is NO OAuth 2.0, NO\n  OpenID Connect and NO API-key surface anywhere in QlikView. Every documented mechanism is\n  either Windows/NTFS identity on the customer's own network or a server-issued short-lived\n  ticket, which is what an on-premises product of this generation looks like.\nderived_from_spec: false\n\
  spec_note: >-\n  derive-authentication.py was not run against a spec because openapi/ is empty; every entry\n  below is quoted from a live 200 documentation page, so method is searched, not derived.\nschemes:\n  - id: qms-service-key\n    type: apiKey\n    in: header\n    name: X-Service-Key\n    applies_to:\n      - QlikView Management API (QMS API)\n      - QlikView Server API\n      - QlikView Distribution Service API (IQDS)\n    description: >-\n      Every QMS API operation must carry a service key in the X-Service-Key HTTP/HTTPS\n      header. The single exception is GetTimeLimitedServiceKey, which is the operation used\n      to OBTAIN a key and therefore cannot require one. Qlik states the header exists to\n      prevent cross-site request forgery.\n    lifetime: >-\n      Time-limited. The key is issued by GetTimeLimitedServiceKey and expires; clients must\n      re-request rather than persist one.\n    obtain_operation: GetTimeLimitedServiceKey\n    transport: SOAP over HTTP\
  \ or HTTPS\n    source: https://help.qlik.com/en-US/qlikview-developer/September2025/Subsystems/QMSAPIref/Content/Home.htm\n  - id: windows-group-authorization\n    type: platform\n    applies_to:\n      - QlikView Management API (QMS API)\n      - QlikView Distribution Service API (IQDS)\n    description: >-\n      Authorization for the QMS API is Windows local-group membership on the QlikView\n      server, not scopes. Most operations require membership of the local group \"QlikView\n      Management API\", which gates overall API access; individual operations additionally\n      require \"QlikView Administrator\" or \"QlikView EDX\".\n    groups:\n      - name: QlikView Management API\n        grants: Overall QMS API access; required by most operations.\n      - name: QlikView Administrator\n        grants: Administrative operations.\n      - name: QlikView EDX\n        grants: External Document Exchange (EDX) task-trigger operations.\n    source: https://help.qlik.com/en-US/qlikview-developer/September2025/Subsystems/QMSAPIref/Content/Home.htm\n\
  \  - id: custom-ticket-exchange\n    type: ticket\n    applies_to:\n      - QlikView Authentication API (Ticket API)\n      - QlikView AccessPoint API\n      - QlikView Workbench API\n    description: >-\n      Custom Ticket Exchange (CTE). A trusted third-party system POSTs a ticket request on\n      behalf of an already-authenticated user; QlikView Server returns a ticket - \"a string\n      of random bytes\" - which the browser then exchanges for a session. This is QlikView's\n      single sign-on path for embedding and for portals that do the authentication themselves.\n    endpoints:\n      - path: /QvAJAXZfc/GetWebTicket.aspx\n        method: POST\n        purpose: Request a ticket for a named user.\n        request_content_type: application/xml\n        request_body_shape: '<Global method=\"GetWebTicket\"><UserId>[User Name]</UserId>[Groups]</Global>'\n        response_body_shape: '<Global><_retval_>[Ticket]</_retval_></Global>'\n      - path: /QvAJAXZfc/Authenticate.aspx\n    \
  \    method: GET\n        purpose: Redirect target that exchanges the ticket for a QlikView session.\n      - path: /Accesspoint.aspx\n        method: POST\n        purpose: Terminate the session (logout).\n    fields:\n      - name: UserId\n        description: The user name the ticket is being minted for.\n        required: true\n      - name: GroupList\n        description: Optional list of group names, each wrapped in a <string> element.\n        required: false\n      - name: GroupsIsNames\n        description: >-\n          true when GroupList carries Document Metadata Service (DMS) group NAMES; false\n          when it carries Windows Security Identifiers (SIDs) for NTFS authorization.\n        required: false\n      - name: Ticket\n        description: The returned random-byte ticket, exchanged at Authenticate.aspx.\n    authorization_modes:\n      - DMS - Document Metadata Service authorization by group name\n      - NTFS - Windows authorization by Security Identifier (SID)\n\
  \    source: https://help.qlik.com/en-US/qlikview-developer/September2025/Content/QV_HelpSites/Ticket-API.htm\n  - id: windows-integrated\n    type: platform\n    applies_to:\n      - QlikView AccessPoint API\n      - QlikView Server API\n    description: >-\n      The default AccessPoint path is Windows integrated authentication (NTLM/Kerberos)\n      against the domain the QlikView Server is joined to, with NTFS or DMS authorization on\n      the documents themselves. No token is exchanged over the API; identity comes from the\n      operating system.\n    source: https://community.qlik.com/t5/Official-Support-Articles/Customized-Authentication-in-QlikView/ta-p/1710763\n  - id: local-com\n    type: none\n    applies_to:\n      - QlikView Plugin API\n      - QlikView OCX API (Automation API)\n      - QlikView QVX SDK API\n    description: >-\n      In-process COM/.NET surfaces on the user's own desktop or server. There is no network\n      authentication because there is no network call\
  \ - the caller already runs as the\n      Windows user.\nnot_present:\n  oauth2: >-\n    QlikView documents no OAuth 2.0 flow of any kind. OAuth on Qlik hosts belongs to Qlik\n    Cloud (qlik.dev), a DIFFERENT product, and is deliberately not recorded here.\n  openid_connect: false\n  jwt: >-\n    Not in QlikView. JWT-based identity providers are a Qlik Sense / Qlik Cloud capability.\n  mutual_tls: >-\n    Not documented for the API surface. QlikView services use certificate trust between\n    their own internal services, which is not a client authentication mechanism.\n  api_keys: >-\n    No developer-portal API key exists; the X-Service-Key value is a server-issued,\n    time-limited session key, not a provisioned credential.\nscopes:\n  model: none\n  note: >-\n    No OAuth scopes exist, so scopes/qlikview-scopes.yml is deliberately NOT written.\n    Authorization is Windows local-group membership plus DMS/NTFS document permissions.\ntransport_security:\n  https_supported: true\n  https_required:\
  \ false\n  note: >-\n    The QMS API accepts SOAP over HTTP or HTTPS; the default installed endpoint is plain\n    HTTP on port 4799. TLS is the customer's deployment choice, not a vendor default, which\n    is a real posture finding for anyone assessing this surface.\nevidence:\n  - url: https://help.qlik.com/en-US/qlikview-developer/September2025/Subsystems/QMSAPIref/Content/Home.htm\n    status: 200\n    fetched: '2026-08-29'\n  - url: https://help.qlik.com/en-US/qlikview-developer/September2025/Content/QV_HelpSites/Ticket-API.htm\n    status: 200\n    fetched: '2026-08-29'\n  - url: https://community.qlik.com/t5/Official-Support-Articles/Customized-Authentication-in-QlikView/ta-p/1710763\n    status: 200\n    fetched: '2026-08-29'\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qlikview/refs/heads/main/authentication/qlikview-authentication.yml
summary_line: 5 schemes
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Discovery
- Data Visualization
- Embedded Analytics
- On-Premises
- SOAP
- Guided Analytics
- Reporting
---
