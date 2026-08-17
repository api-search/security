---
api_key_in:
- body
- header
- query
auth_types:
- hmac-signature
- http-basic
- credentials-in-payload
- ws-security-usernametoken
- mutualTLS
- saml2-sso
description: ''
kind: authentication
layout: security
method: searched
name: Waystar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Waystar secures its APIs with hmac-signature, http-basic, credentials-in-payload, ws-security-usernametoken, mutualTLS, and saml2-sso across 9 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Waystar
provider_slug: waystar
scheme_count: 9
schemes:
- algorithm: HMAC-SHA1
  applies_to:
  - Claims Web Services (claimsapi.zirmed.com)
  - Remittance / EOB Web Service (remitsapi.waystar.com)
  - Statements / Print Services (printservices.zirmed.com)
  - ZPay payment transactions (zpayapi.zirmed.com)
  - Legacy ServiceHandler (www.zirmed.com/Services/ServiceHandler.ashx)
  canonicalization: Sort the non-empty key/value pairs in case-insensitive alphabetical order, concatenate keys and values into a single string with the "&" and "=" delimiters removed, then HMAC-SHA1 that string with the client's HMAC Key and Base64-encode the result. Append it to the POST data as the "Signature" key.
  encoding: base64
  failure: A signature mismatch returns "401 Not Authorized" and the call is not processed further.
  in: body
  key_issuance: HMAC keys are issued per client by Waystar. Test keys are requested from apisupport@waystar.com.
  name: WaystarHMAC-SHA1
  parameter: Signature
  source: https://developer.waystar.com/documents/integration-basics/hmac-security-for-web-services-api-information/
  type: hmac-signature
- algorithm: HMAC-SHA256
  applies_to:
  - Patient Estimation API (estimationapi.zirmed.com/1.0)
  canonicalization: Concatenate, with no separators - (1) the request method (GET or POST), (2) the full request URI lowercased including query string, (3) the Date header value in yyyy-MM-ddTHH:mm:ss UTC form, (4) the CustID, (5) the Base64-encoded request body. HMAC-SHA256 the UTF-8 representation with the UTF-8 WebCallEncryptionKey, Base64 the digest.
  encoding: base64
  header_format: HMAC <CustID>:<base64 signature>
  in: header
  key_name: WebCallEncryptionKey
  name: WaystarHMAC-SHA256
  parameter: Authorization
  required_headers:
  - format: RFC 1123 UTC (e.g. 'Mon, 12 Jan 2015 20:50:07 GMT')
    name: Date
    note: Replay window - a POST is rejected unless its UTC timestamp is within +/- 30 seconds of Waystar's clock.
  scheme_prefix: HMAC
  source: https://developer.waystar.com/documents/patient-access/patient-estimation/
  type: hmac-signature
- applies_to:
  - Eligibility REST Gateway (eligibilityapi.zirmed.com/1.0/Rest/Gateway/GatewayAsync.ashx)
  in: body
  name: RealTimeAPICredentials
  note: The eligibility REST gateway takes the RealTime API UserID and Password as POST form fields alongside the inquiry payload rather than as a header. A bad username/password returns the error message "Authentication Failure".
  parameters:
  - UserID
  - Password
  source: https://developer.waystar.com/documents/patient-access/insurance-verification/
  type: credentials-in-payload
- applies_to:
  - Credential Management API (login.zirmed.com/RealTimeExternal/1.0/api/password/changepassword)
  - Prior Authorization API (priorauthorizationapi.waystar.com/1.0)
  in: header
  name: BasicAuth
  note: The RealTime External Credential Management API requires a valid RealTime API user passed with HTTP Basic Auth. The user must additionally hold the "Allow FTP Whitelisting" permission to rotate an SFTP password, and must have permission on the supplied CustId.
  scheme: basic
  source: https://developer.waystar.com/documents/integration-basics/credential-management-api/
  type: http
- applies_to:
  - Real-time claim status 276/277 (claimsapi.zirmed.com/ExternalClaimStatus/ExternalCSIntake/Process)
  - Immediate Claims 837 intake (claimsapi.zirmed.com/ImmediateClaims/Intake/Process)
  in: soap-header
  name: WSSecurityUsernameToken
  profile: The 276/277 endpoint uses the OASIS WS-Security 1.0 UsernameToken profile inside a CAQH CORE Rule 2.2.0 SOAP envelope. The ImmediateClaims endpoint uses a Waystar-proprietary <SecurityHeaderElement> carrying <Username> and <Password>. XML element names are case sensitive.
  source: https://developer.waystar.com/documents/claim-and-denial-management/claim-management-2/
  type: ws-security-usernametoken
- applies_to:
  - Eligibility SOAP (eligibilityapi.zirmed.com/1.0/Soap/CoreSoapAPI.svc/x509)
  name: X509ClientCertificate
  note: Waystar exposes a separate SOAP endpoint suffixed /x509 for client-certificate authentication, per the CAQH CORE Phase II Connectivity Rule (envelope standard B).
  source: https://developer.waystar.com/documents/patient-access/insurance-verification/
  type: mutualTLS
- applies_to:
  - Waystar portal single sign-on (www.waystar.com)
  name: SAML2-SSO
  note: Waystar acts as the SAML 2.0 Service Provider; the client system is the Identity Provider. Supports SP-initiated web SSO, W3C XML encryption, deep linking to a specific portal URL, and programmatic creation/update of Waystar portal users, roles, account access and default account.
  source: https://developer.waystar.com/documents/integration-basics/sso/
  type: saml2
  version: '2.0'
- applies_to:
  - Seamless portal login handoff
  endpoint: https://www.zirmed.com/private/vallogin.aspx
  in: body
  name: DirectedWaystarLogin
  note: Waystar states explicitly that the HMAC signature is NOT used or supported on this call - security rests entirely on the login/password pair, so it must be POSTed and never issued as a GET.
  parameters:
  - LoginName
  - Password
  - URLRedirect
  source: https://developer.waystar.com/documents/integration-basics/directed-waystar-login/
  type: credentials-in-payload
- host: sshftp.waystar.com
  name: SFTPCredentials
  note: Batch/file services authenticate with an SFTP login and password issued by the Waystar implementation project manager. Waystar blocks/blacklists any IP address after 5 consecutive unsuccessful connection attempts. FTP passwords can be rotated through the Credential Management API.
  source: https://developer.waystar.com/documents/integration-basics/ssh-ftp-instructions/
  type: sftp
slug: waystar-authentication
source_filename: waystar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://developer.waystar.com/documents/integration-basics/\ndocs:\n- https://developer.waystar.com/documents/integration-basics/hmac-security-for-web-services-api-information/\n- https://developer.waystar.com/documents/integration-basics/credential-management-api/\n- https://developer.waystar.com/documents/integration-basics/sso/\n- https://developer.waystar.com/documents/integration-basics/directed-waystar-login/\n- https://developer.waystar.com/documents/patient-estimation/\n- https://developer.waystar.com/documents/patient-access/patient-estimation/\n- https://developer.waystar.com/documents/patient-access/insurance-verification/\n- https://developer.waystar.com/documents/claim-and-denial-management/claim-management/\nprovider: Waystar\nproviderId: waystar\nnote: >-\n  Waystar does not publish an OpenAPI definition, so this profile is read\n  directly from the Waystar developer-portal documentation rather than derived\n\
  \  from securitySchemes. Waystar runs SIX distinct authentication models across\n  its API surface - they are not interchangeable, and which one applies depends\n  entirely on which product API is being called. Note the correction: the\n  original Waystar Developer Suite HMAC signature is HMAC-SHA1 Base64 (not\n  SHA256); only the newer Estimation API uses HMAC-SHA256. Getting this wrong\n  produces a 401 on every call.\nsummary:\n  types: [hmac-signature, http-basic, credentials-in-payload, ws-security-usernametoken, mutualTLS, saml2-sso]\n  api_key_in: [body, header, query]\n  oauth2_flows: []\n  oauth2_supported: false\n  openid_connect: false\n  identity_unit: >-\n    CustID - a hierarchical Waystar customer identifier. Each client has a CustID;\n    each facility/site of that client also has a CustID and can be grouped under\n    the client. One HMAC key is issued per client and is valid for all of that\n    client's facilities.\nschemes:\n- name: WaystarHMAC-SHA1\n  type: hmac-signature\n\
  \  algorithm: HMAC-SHA1\n  encoding: base64\n  in: body\n  parameter: Signature\n  applies_to:\n  - Claims Web Services (claimsapi.zirmed.com)\n  - Remittance / EOB Web Service (remitsapi.waystar.com)\n  - Statements / Print Services (printservices.zirmed.com)\n  - ZPay payment transactions (zpayapi.zirmed.com)\n  - Legacy ServiceHandler (www.zirmed.com/Services/ServiceHandler.ashx)\n  canonicalization: >-\n    Sort the non-empty key/value pairs in case-insensitive alphabetical order,\n    concatenate keys and values into a single string with the \"&\" and \"=\"\n    delimiters removed, then HMAC-SHA1 that string with the client's HMAC Key and\n    Base64-encode the result. Append it to the POST data as the \"Signature\" key.\n  failure: >-\n    A signature mismatch returns \"401 Not Authorized\" and the call is not\n    processed further.\n  key_issuance: >-\n    HMAC keys are issued per client by Waystar. Test keys are requested from\n    apisupport@waystar.com.\n  source: https://developer.waystar.com/documents/integration-basics/hmac-security-for-web-services-api-information/\n\
  - name: WaystarHMAC-SHA256\n  type: hmac-signature\n  algorithm: HMAC-SHA256\n  encoding: base64\n  in: header\n  parameter: Authorization\n  scheme_prefix: HMAC\n  header_format: 'HMAC <CustID>:<base64 signature>'\n  applies_to:\n  - Patient Estimation API (estimationapi.zirmed.com/1.0)\n  canonicalization: >-\n    Concatenate, with no separators - (1) the request method (GET or POST), (2)\n    the full request URI lowercased including query string, (3) the Date header\n    value in yyyy-MM-ddTHH:mm:ss UTC form, (4) the CustID, (5) the Base64-encoded\n    request body. HMAC-SHA256 the UTF-8 representation with the UTF-8\n    WebCallEncryptionKey, Base64 the digest.\n  required_headers:\n  - name: Date\n    format: RFC 1123 UTC (e.g. 'Mon, 12 Jan 2015 20:50:07 GMT')\n    note: >-\n      Replay window - a POST is rejected unless its UTC timestamp is within\n      +/- 30 seconds of Waystar's clock.\n  key_name: WebCallEncryptionKey\n  source: https://developer.waystar.com/documents/patient-access/patient-estimation/\n\
  - name: RealTimeAPICredentials\n  type: credentials-in-payload\n  in: body\n  parameters: [UserID, Password]\n  applies_to:\n  - Eligibility REST Gateway (eligibilityapi.zirmed.com/1.0/Rest/Gateway/GatewayAsync.ashx)\n  note: >-\n    The eligibility REST gateway takes the RealTime API UserID and Password as\n    POST form fields alongside the inquiry payload rather than as a header. A bad\n    username/password returns the error message \"Authentication Failure\".\n  source: https://developer.waystar.com/documents/patient-access/insurance-verification/\n- name: BasicAuth\n  type: http\n  scheme: basic\n  in: header\n  applies_to:\n  - Credential Management API (login.zirmed.com/RealTimeExternal/1.0/api/password/changepassword)\n  - Prior Authorization API (priorauthorizationapi.waystar.com/1.0)\n  note: >-\n    The RealTime External Credential Management API requires a valid RealTime API\n    user passed with HTTP Basic Auth. The user must additionally hold the \"Allow\n    FTP Whitelisting\"\
  \ permission to rotate an SFTP password, and must have\n    permission on the supplied CustId.\n  source: https://developer.waystar.com/documents/integration-basics/credential-management-api/\n- name: WSSecurityUsernameToken\n  type: ws-security-usernametoken\n  in: soap-header\n  applies_to:\n  - Real-time claim status 276/277 (claimsapi.zirmed.com/ExternalClaimStatus/ExternalCSIntake/Process)\n  - Immediate Claims 837 intake (claimsapi.zirmed.com/ImmediateClaims/Intake/Process)\n  profile: >-\n    The 276/277 endpoint uses the OASIS WS-Security 1.0 UsernameToken profile\n    inside a CAQH CORE Rule 2.2.0 SOAP envelope. The ImmediateClaims endpoint\n    uses a Waystar-proprietary <SecurityHeaderElement> carrying <Username> and\n    <Password>. XML element names are case sensitive.\n  source: https://developer.waystar.com/documents/claim-and-denial-management/claim-management-2/\n- name: X509ClientCertificate\n  type: mutualTLS\n  applies_to:\n  - Eligibility SOAP (eligibilityapi.zirmed.com/1.0/Soap/CoreSoapAPI.svc/x509)\n\
  \  note: >-\n    Waystar exposes a separate SOAP endpoint suffixed /x509 for client-certificate\n    authentication, per the CAQH CORE Phase II Connectivity Rule (envelope\n    standard B).\n  source: https://developer.waystar.com/documents/patient-access/insurance-verification/\n- name: SAML2-SSO\n  type: saml2\n  version: '2.0'\n  applies_to:\n  - Waystar portal single sign-on (www.waystar.com)\n  note: >-\n    Waystar acts as the SAML 2.0 Service Provider; the client system is the\n    Identity Provider. Supports SP-initiated web SSO, W3C XML encryption, deep\n    linking to a specific portal URL, and programmatic creation/update of Waystar\n    portal users, roles, account access and default account.\n  source: https://developer.waystar.com/documents/integration-basics/sso/\n- name: DirectedWaystarLogin\n  type: credentials-in-payload\n  in: body\n  parameters: [LoginName, Password, URLRedirect]\n  endpoint: https://www.zirmed.com/private/vallogin.aspx\n  applies_to:\n  - Seamless\
  \ portal login handoff\n  note: >-\n    Waystar states explicitly that the HMAC signature is NOT used or supported on\n    this call - security rests entirely on the login/password pair, so it must be\n    POSTed and never issued as a GET.\n  source: https://developer.waystar.com/documents/integration-basics/directed-waystar-login/\n- name: SFTPCredentials\n  type: sftp\n  host: sshftp.waystar.com\n  note: >-\n    Batch/file services authenticate with an SFTP login and password issued by the\n    Waystar implementation project manager. Waystar blocks/blacklists any IP\n    address after 5 consecutive unsuccessful connection attempts. FTP passwords\n    can be rotated through the Credential Management API.\n  source: https://developer.waystar.com/documents/integration-basics/ssh-ftp-instructions/\ncredential_rotation:\n  supported: true\n  endpoint: https://login.zirmed.com/RealTimeExternal/1.0/api/password/changepassword\n  auth: http-basic\n  operations:\n    '1': FTP password only\n\
  \    '2': RealTime API password only\n    '3': both\n  note: >-\n    Waystar publishes a first-party credential-rotation API - uncommon in this\n    sector and a genuine agent-relevant capability, since a long-lived integration\n    can rotate its own API and SFTP secrets programmatically.\ntransport_security:\n  tls: required\n  note: >-\n    Waystar states all HTTPS web service calls use up to 2048-bit RSA encryption.\n  source: https://developer.waystar.com/documents/integration-basics/privacy-and-security/\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waystar/refs/heads/main/authentication/waystar-authentication.yml
summary_line: hmac-signature/http-basic/credentials-in-payload/ws-security-usernametoken/mutualTLS/saml2-sso · 9 schemes
tags:
- Healthcare
- Revenue Cycle Management
- RCM
- Clearinghouse
- Healthcare Payments
- Medical Billing
- X12 EDI
- Eligibility
- Claims
- Remittance
---
