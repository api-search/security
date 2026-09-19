---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'Authentication profile for Novell''s two callable API surfaces, read from the GroupWise 25 SDK documentation still served on www.novell.com. Both surfaces are customer-hosted and both authenticate against the customer''s own GroupWise system - there is no Novell-operated identity provider, no API key issuance, no OAuth authorization server and no OpenID Connect discovery document anywhere on the Novell domain (every /.well-known/ probe 404d; see well-known/novell-well-known.yml). The strongest credential on offer is the GroupWise Trusted Application key, which is a system-wide impersonation credential minted by the customer''s own GroupWise administrator. DERIVED FROM DOCUMENTATION, NOT A SPEC: no OpenAPI, WSDL or other machine-readable contract could be obtained for either surface, so there is no securitySchemes block behind this file.'
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Novell Authentication
name_suffix: Authentication
oauth_flows: []
overview: Novell declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Novell
provider_slug: novell
scheme_count: 4
schemes:
- api: novell:groupwise-web-services-soap
  description: loginRequest carries a types:auth element of type PlainText containing the GroupWise username and password. There is no separate authorization header; the credential travels inside the SOAP body.
  example_shape: "<loginRequest>\n  <types:auth types:PlainText>\n    <username>...</username>\n    <password>...</password>\n  <auth/>\n  <application>...</application>\n</loginRequest>\n"
  id: groupwise-soap-plaintext
  session:
    description: loginResponse returns a session key that every subsequent method must carry for the life of the session. loginRequest must be the first call; no other method may be invoked before it.
    idle_timeout_minutes: 30
    keepalive: getTimestampRequest accepts a noop parameter that holds both the GroupWise session and the HTTP keep-alive connection open.
    mechanism: session key
    termination: logoutRequest
  source: https://www.novell.com/documentation/groupwise25/gwsdk_web_services/data/b7m3i3q.html
  transport: SOAP over HTTP or HTTPS
  transport_security:
    https_available: true
    https_default: false
    note: HTTPS is supported but must be explicitly enabled per POA ("each POA needs to have SSL connections enabled for SOAP"). Because the password is in the request body, a POA left on plain HTTP transmits GroupWise credentials in cleartext. This is a deployment decision made by the customer, not a property of the protocol.
  type: credential-in-body
- api: novell:groupwise-web-services-soap
  blast_radius: System-wide. A trusted application key grants mailbox read and write access to every account in the GroupWise system. It is the highest-privilege credential this API has and there is no documented scope, audience or per-mailbox restriction on it.
  description: A Trusted Application logs in to ANY account in the GroupWise system without knowing that user's password. The GroupWise administrator creates a trusted application name and key and decides which applications may use it; the application passes the name and key to loginRequest in place of a user credential.
  id: groupwise-trusted-application
  reference: https://www.novell.com/documentation/developer/groupwise_sdk/gwsdk_gwtapp/data/bktitle.html
  rotation: Not documented. Revocation is administrative - the GroupWise administrator removes or disables the trusted application entry.
  scopes: none
  source: https://www.novell.com/documentation/groupwise25/gwsdk_web_services/data/b7m3i43.html
  type: shared-secret impersonation
- api: novell:groupwise-administration-rest-api
  description: The Admin REST API exposes gw-api/system/login, gw-api/system/login/{path} and gw-api/system/logout as its session endpoints, and the shipped sample code is configured with a URL, an admin user name and a password in src/main/resources/config.properties. The credential is therefore a GroupWise administrator account on the customer's own system.
  id: groupwise-admin-rest-login
  per_admin_scoping:
    documented: true
    note: gw-api/async filters the job list to jobs submitted by the admin making the request, which confirms the service tracks caller identity per administrator rather than treating all callers as one principal.
  recover_connection:
    note: gw-api/system/login/{path} creates a read-only "Recover" connection to a backup copy of a domain database - a distinct, deliberately read-only authentication mode.
  scopes: none
  source: https://www.novell.com/documentation/developer/groupwise_sdk/gwsdk_gwadminweb/data/application.htm
  type: session
- api: novell:dsml-for-edirectory-soap
  description: DSML for eDirectory is a servlet the customer deploys in front of their own eDirectory tree; the identity that matters is the eDirectory LDAP bind behind it. Simple bind and SASL are eDirectory features, not properties Novell documents at the DSML layer.
  id: edirectory-ldap-bind
  source: https://www.microfocus.com/documentation/edirectory-developer-documentation/dsml-for-edirectory-soap/
  type: ldap-bind
slug: novell-authentication
source_filename: novell-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: searched\nsource: https://www.novell.com/documentation/groupwise25/gwsdk_web_services/data/b7m3i3i.html\nname: Novell API authentication\ndescription: >-\n  Authentication profile for Novell's two callable API surfaces, read from the GroupWise 25 SDK documentation\n  still served on www.novell.com. Both surfaces are customer-hosted and both authenticate against the\n  customer's own GroupWise system - there is no Novell-operated identity provider, no API key issuance, no\n  OAuth authorization server and no OpenID Connect discovery document anywhere on the Novell domain (every\n  /.well-known/ probe 404d; see well-known/novell-well-known.yml). The strongest credential on offer is the\n  GroupWise Trusted Application key, which is a system-wide impersonation credential minted by the customer's\n  own GroupWise administrator.\n  DERIVED FROM DOCUMENTATION, NOT A SPEC: no OpenAPI, WSDL or other machine-readable contract could be\n  obtained for\
  \ either surface, so there is no securitySchemes block behind this file.\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_keys_issued_by_provider: false\nschemes:\n  - id: groupwise-soap-plaintext\n    api: novell:groupwise-web-services-soap\n    type: credential-in-body\n    transport: SOAP over HTTP or HTTPS\n    description: >-\n      loginRequest carries a types:auth element of type PlainText containing the GroupWise username and\n      password. There is no separate authorization header; the credential travels inside the SOAP body.\n    example_shape: |\n      <loginRequest>\n        <types:auth types:PlainText>\n          <username>...</username>\n          <password>...</password>\n        <auth/>\n        <application>...</application>\n      </loginRequest>\n    session:\n      mechanism: session key\n      description: >-\n        loginResponse returns a session key that every subsequent method must carry for the life of the\n        session. loginRequest must be\
  \ the first call; no other method may be invoked before it.\n      idle_timeout_minutes: 30\n      keepalive: >-\n        getTimestampRequest accepts a noop parameter that holds both the GroupWise session and the HTTP\n        keep-alive connection open.\n      termination: logoutRequest\n    transport_security:\n      https_available: true\n      https_default: false\n      note: >-\n        HTTPS is supported but must be explicitly enabled per POA (\"each POA needs to have SSL connections\n        enabled for SOAP\"). Because the password is in the request body, a POA left on plain HTTP transmits\n        GroupWise credentials in cleartext. This is a deployment decision made by the customer, not a\n        property of the protocol.\n    source: https://www.novell.com/documentation/groupwise25/gwsdk_web_services/data/b7m3i3q.html\n  - id: groupwise-trusted-application\n    api: novell:groupwise-web-services-soap\n    type: shared-secret impersonation\n    description: >-\n      A Trusted\
  \ Application logs in to ANY account in the GroupWise system without knowing that user's\n      password. The GroupWise administrator creates a trusted application name and key and decides which\n      applications may use it; the application passes the name and key to loginRequest in place of a user\n      credential.\n    blast_radius: >-\n      System-wide. A trusted application key grants mailbox read and write access to every account in the\n      GroupWise system. It is the highest-privilege credential this API has and there is no documented scope,\n      audience or per-mailbox restriction on it.\n    scopes: none\n    rotation: >-\n      Not documented. Revocation is administrative - the GroupWise administrator removes or disables the\n      trusted application entry.\n    source: https://www.novell.com/documentation/groupwise25/gwsdk_web_services/data/b7m3i43.html\n    reference: https://www.novell.com/documentation/developer/groupwise_sdk/gwsdk_gwtapp/data/bktitle.html\n  - id:\
  \ groupwise-admin-rest-login\n    api: novell:groupwise-administration-rest-api\n    type: session\n    description: >-\n      The Admin REST API exposes gw-api/system/login, gw-api/system/login/{path} and gw-api/system/logout as\n      its session endpoints, and the shipped sample code is configured with a URL, an admin user name and a\n      password in src/main/resources/config.properties. The credential is therefore a GroupWise administrator\n      account on the customer's own system.\n    per_admin_scoping:\n      documented: true\n      note: >-\n        gw-api/async filters the job list to jobs submitted by the admin making the request, which confirms\n        the service tracks caller identity per administrator rather than treating all callers as one\n        principal.\n    recover_connection:\n      note: >-\n        gw-api/system/login/{path} creates a read-only \"Recover\" connection to a backup copy of a domain\n        database - a distinct, deliberately read-only authentication\
  \ mode.\n    scopes: none\n    source: https://www.novell.com/documentation/developer/groupwise_sdk/gwsdk_gwadminweb/data/application.htm\n  - id: edirectory-ldap-bind\n    api: novell:dsml-for-edirectory-soap\n    type: ldap-bind\n    description: >-\n      DSML for eDirectory is a servlet the customer deploys in front of their own eDirectory tree; the\n      identity that matters is the eDirectory LDAP bind behind it. Simple bind and SASL are eDirectory\n      features, not properties Novell documents at the DSML layer.\n    source: https://www.microfocus.com/documentation/edirectory-developer-documentation/dsml-for-edirectory-soap/\ndiscovery_documents:\n  openid_configuration: null\n  oauth_authorization_server: null\n  oauth_protected_resource: null\n  note: >-\n    All three probed 404 on www.novell.com and are unreachable on the apex (TLS SAN mismatch). The only\n    identity provider on any Novell-branded host is extlogin.opentext.com, an OpenText SAML 2.0 SSO endpoint\n    that\
  \ fronts support.novell.com and the Micro Focus support portal - it gates OpenText customer support,\n    not these APIs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/novell/refs/heads/main/authentication/novell-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Enterprise Software
- Collaboration
- Email
- Directory Services
- Identity
- groupware
- LDAP
- SOAP
- Legacy
- Self-Hosted
- Endpoint Management
---
