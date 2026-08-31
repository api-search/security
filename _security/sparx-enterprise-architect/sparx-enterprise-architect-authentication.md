---
api_key_in:
- header
auth_types:
- http
- custom-token
- openIdConnect
- ntlm
description: ''
kind: authentication
layout: security
method: searched
name: Sparx Enterprise Architect Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Sparx Enterprise Architect secures its APIs with http, custom-token, openIdConnect, and ntlm across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Sparx Enterprise Architect
provider_slug: sparx-enterprise-architect
scheme_count: 6
schemes:
- description: Every OSLC GET/POST is rejected by Pro Cloud Server unless a user authentication token is supplied. The token is obtained by POSTing to the login endpoint and is returned inside the RDF/XML response as the element ss:useridentifier.
  in: query
  name: OSLCUserAuthenticationToken
  obtain:
    endpoint: <protocol>://<server>/<model_name>/oslc/am/login/
    method: POST
    response_also_returns:
    - ss:readonlymodel — whether the model permits resource creation/update
    - ss:validlicense — whether a valid Pro Cloud Server licence is present
    - ss:userfullname — foaf:Person with foaf:name and foaf:nick
    - ss:accesstoken — OpenID access token, OpenID-authenticated models only
    - ss:refreshtoken — OpenID refresh token, OpenID-authenticated models only
    - ss:elementpermission — permission to create/update resources
    response_media_type: application/rdf+xml
    response_token_element: ss:useridentifier
  parameter: useridentifier
  revoke:
    endpoint: <protocol>://<server>/<model_name>/oslc/am/logout/?useridentifier=<token>
    method: GET
  type: custom-token
- description: For a project with Enterprise Architect model security enabled, the client POSTs the same user ID and password used to open the secured project.
  name: EnterpriseArchitectModelSecurity
  request:
    body: uid=<USER ID>;pwd=<PASSWORD>;
    endpoint: <protocol>://<server>/<model_name>/oslc/am/login/
    method: POST
  scheme: form-post-credentials
  type: http
- description: For a project with model security disabled a token is still required, but it can be requested with empty credentials.
  name: NoSecurityLogin
  request:
    body: uid=;pwd=;
    endpoint: <protocol>://<server>/<model_name>/oslc/am/login/
    method: POST
  scheme: form-post-credentials
  type: http
- description: Windows NTLM single sign-on against the Pro Cloud Server.
  name: NTLM
  request:
    body: sso=ntlm;
    endpoint: <protocol>://<server>/<model_name>/oslc/am/login/
    method: POST
  scheme: ntlm
  type: http
- description: For OpenID-enabled projects the client first authenticates the user at the authorizationURI endpoint named in the Service Provider Resource, then exchanges the resulting authorization code and redirect URI for a Sparx user authentication token. The identity provider is configured per Pro Cloud Server deployment, so there is no vendor-published discovery document or fixed scope list.
  flows:
  - authorizationUrl: advertised per deployment in the OSLC Service Provider Resource (<protocol>://<server>/<model_name>/oslc/am/sp/)
    flow: authorizationCode
    scopes: {}
    scopes_note: No scope list is published. Authorisation is expressed through Enterprise Architect model security permissions (ss:elementpermission, ss:diagrampermission, ss:readonlymodel) returned at login, not through OAuth scopes. No scopes/ artifact is emitted for that reason.
    tokenUrl: <protocol>://<server>/<model_name>/oslc/am/login/
  name: OpenIDConnect
  request:
    body: sso=openid;code=<AUTHORIZATION CODE>;redirecturi=<REDIRECT URI>;
    endpoint: <protocol>://<server>/<model_name>/oslc/am/login/
    method: POST
  type: openIdConnect
- description: An optional shared access code configured per project in the Pro Cloud Server configuration tool. When set, the client must send it as the custom HTTP header EAO-Access-Code on every OSLC request; Pro Cloud Server validates it before processing the request. This layers on top of, and does not replace, the user authentication token.
  in: header
  name: EAOAccessCode
  parameter: EAO-Access-Code
  source: https://www.sparxsystems.jp/help/17.0/oslc_access_code.html
  type: apiKey
slug: sparx-enterprise-architect-authentication
source_filename: sparx-enterprise-architect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://www.sparxsystems.jp/help/17.0/oslc_user_cred.html\ndocs: https://www.sparxsystems.jp/help/17.0/oslc_user_cred.html\nalso_see:\n  - https://www.sparxsystems.jp/help/17.0/oslc_access_code.html\n  - https://www.sparxsystems.jp/help/17.0/oslc_serv_provid.html\nsource_note: >-\n  The canonical English pages for these topics live at\n  sparxsystems.com/enterprise_architect_user_guide/17.x/the_model_repository/oslc_user_cred.html\n  and oslc_access_code.html, but sparxsystems.com serves a Cloudflare managed challenge (HTTP 403)\n  to non-browser clients. The identical topics were read from the Sparx Systems Japan help mirror\n  (www.sparxsystems.jp/help/17.0/), which is served by a Sparx Systems entity and carries the same\n  URLs, headers and RDF payloads verbatim.\nsummary:\n  types: [http, custom-token, openIdConnect, ntlm]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  applies_to: Pro Cloud Server OSLC\
  \ RESTful API (the only HTTP API surface)\n  note: >-\n    The COM Automation Interface, Add-In Framework and scripting engine are in-process surfaces\n    inside a licensed Enterprise Architect installation. They have no network authentication; the\n    security boundary is the Windows session plus, optionally, Enterprise Architect's own model\n    security (user ID / password) when the project has security enabled.\nschemes:\n  - name: OSLCUserAuthenticationToken\n    type: custom-token\n    in: query\n    parameter: useridentifier\n    description: >-\n      Every OSLC GET/POST is rejected by Pro Cloud Server unless a user authentication token is\n      supplied. The token is obtained by POSTing to the login endpoint and is returned inside the\n      RDF/XML response as the element ss:useridentifier.\n    obtain:\n      endpoint: '<protocol>://<server>/<model_name>/oslc/am/login/'\n      method: POST\n      response_media_type: application/rdf+xml\n      response_token_element: 'ss:useridentifier'\n\
  \      response_also_returns:\n        - 'ss:readonlymodel — whether the model permits resource creation/update'\n        - 'ss:validlicense — whether a valid Pro Cloud Server licence is present'\n        - 'ss:userfullname — foaf:Person with foaf:name and foaf:nick'\n        - 'ss:accesstoken — OpenID access token, OpenID-authenticated models only'\n        - 'ss:refreshtoken — OpenID refresh token, OpenID-authenticated models only'\n        - 'ss:elementpermission — permission to create/update resources'\n    revoke:\n      endpoint: '<protocol>://<server>/<model_name>/oslc/am/logout/?useridentifier=<token>'\n      method: GET\n  - name: EnterpriseArchitectModelSecurity\n    type: http\n    scheme: form-post-credentials\n    description: >-\n      For a project with Enterprise Architect model security enabled, the client POSTs the same\n      user ID and password used to open the secured project.\n    request:\n      endpoint: '<protocol>://<server>/<model_name>/oslc/am/login/'\n   \
  \   method: POST\n      body: 'uid=<USER ID>;pwd=<PASSWORD>;'\n  - name: NoSecurityLogin\n    type: http\n    scheme: form-post-credentials\n    description: >-\n      For a project with model security disabled a token is still required, but it can be\n      requested with empty credentials.\n    request:\n      endpoint: '<protocol>://<server>/<model_name>/oslc/am/login/'\n      method: POST\n      body: 'uid=;pwd=;'\n  - name: NTLM\n    type: http\n    scheme: ntlm\n    description: Windows NTLM single sign-on against the Pro Cloud Server.\n    request:\n      endpoint: '<protocol>://<server>/<model_name>/oslc/am/login/'\n      method: POST\n      body: 'sso=ntlm;'\n  - name: OpenIDConnect\n    type: openIdConnect\n    description: >-\n      For OpenID-enabled projects the client first authenticates the user at the authorizationURI\n      endpoint named in the Service Provider Resource, then exchanges the resulting authorization\n      code and redirect URI for a Sparx user authentication\
  \ token. The identity provider is\n      configured per Pro Cloud Server deployment, so there is no vendor-published discovery\n      document or fixed scope list.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: 'advertised per deployment in the OSLC Service Provider Resource (<protocol>://<server>/<model_name>/oslc/am/sp/)'\n        tokenUrl: '<protocol>://<server>/<model_name>/oslc/am/login/'\n        scopes: {}\n        scopes_note: >-\n          No scope list is published. Authorisation is expressed through Enterprise Architect model\n          security permissions (ss:elementpermission, ss:diagrampermission, ss:readonlymodel)\n          returned at login, not through OAuth scopes. No scopes/ artifact is emitted for that\n          reason.\n    request:\n      endpoint: '<protocol>://<server>/<model_name>/oslc/am/login/'\n      method: POST\n      body: 'sso=openid;code=<AUTHORIZATION CODE>;redirecturi=<REDIRECT URI>;'\n  - name: EAOAccessCode\n    type: apiKey\n\
  \    in: header\n    parameter: EAO-Access-Code\n    description: >-\n      An optional shared access code configured per project in the Pro Cloud Server configuration\n      tool. When set, the client must send it as the custom HTTP header EAO-Access-Code on every\n      OSLC request; Pro Cloud Server validates it before processing the request. This layers on top\n      of, and does not replace, the user authentication token.\n    source: https://www.sparxsystems.jp/help/17.0/oslc_access_code.html\nlicensing_gate: >-\n  The OSLC RESTful API is available only on a Pro Cloud Server with a paid licence applied. An\n  unlicensed Pro Cloud Server provides secure cloud repository connections and floating licences\n  but not OSLC.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sparx-enterprise-architect/refs/heads/main/authentication/sparx-enterprise-architect-authentication.yml
summary_line: http/custom-token/openIdConnect/ntlm · 6 schemes
tags:
- Enterprise Architecture
- Modeling
- Software Engineering
- Systems Engineering
- UML
- ArchiMate
- BPMN
- SysML
- OSLC
- MCP
- Model-Driven Development
---
