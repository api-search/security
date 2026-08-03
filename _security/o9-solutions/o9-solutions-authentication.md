---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: O9 Solutions Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: o9 Solutions secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: o9 Solutions
provider_slug: o9-solutions
scheme_count: 1
schemes:
- clients_observed:
  - client_id: c9fd4e6a-498d-43e9-aedc-3cf50d254308
    name: o9 Platform Wiki
    redirect_uri: https://platformwiki.o9solutions.com/index.php/Special:OAuth2Client/callback
    scope: openid email profile
  - client_id: c3efaf96-a57c-48dd-a58d-f07e871b8ba9
    name: o9 Community
    redirect_uri: https://community.o9solutions.com/auth/oauth2_basic/callback
    scope: ''
  discovery:
    oauth_authorization_server: not published (404)
    openid_configuration: not published (404 at /.well-known/openid-configuration and /oauthserver/.well-known/openid-configuration)
  flows:
  - authorizationUrl: https://guide.o9solutions.com/oauthserver/authorize
    flow: authorizationCode
    response_mode: observed as empty or a target-page token (e.g. RedirectToApiDocs)
    response_type: code
    scopes_observed:
    - openid
    - email
    - profile
  identity_providers:
  - audience: business email accounts (customers and partners)
    endpoint: https://guide.o9solutions.com/OAuth/AzureB2C
    mfa: observed isMFAEnabled=True on the authorize request
    name: Azure AD B2C
  - audience: o9 employees (SSO)
    endpoint: https://guide.o9solutions.com/OAuth/MicrosoftOrganizationAccount
    name: Microsoft Organization Account
  name: o9 OAuth 2.0 (guide.o9solutions.com/oauthserver)
  type: oauth2
slug: o9-solutions-authentication
source_filename: o9-solutions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: https://guide.o9solutions.com/oauthserver/authorize\ndocs: https://guide.o9solutions.com/Resources/ApiDocs\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  api_key_in: []\n  public_api_auth_documentation: gated\n  note: >-\n    o9 publishes no public OpenAPI, so this profile is NOT derived from a\n    machine-readable contract. It records the authentication surface that is\n    directly observable without an account: o9 operates its own OAuth 2.0\n    authorization server at guide.o9solutions.com/oauthserver, and every o9\n    developer property (the API guide, the platform wiki, the community, the\n    documentation portal) is a client of it. The authentication contract for\n    the o9 Platform API and Reference Model API themselves is documented behind\n    that gate and is not publicly retrievable.\nschemes:\n- name: o9 OAuth 2.0 (guide.o9solutions.com/oauthserver)\n  type: oauth2\n  flows:\n  - flow:\
  \ authorizationCode\n    authorizationUrl: https://guide.o9solutions.com/oauthserver/authorize\n    scopes_observed:\n    - openid\n    - email\n    - profile\n    response_type: code\n    response_mode: observed as empty or a target-page token (e.g. RedirectToApiDocs)\n  identity_providers:\n  - name: Azure AD B2C\n    endpoint: https://guide.o9solutions.com/OAuth/AzureB2C\n    audience: business email accounts (customers and partners)\n    mfa: observed isMFAEnabled=True on the authorize request\n  - name: Microsoft Organization Account\n    endpoint: https://guide.o9solutions.com/OAuth/MicrosoftOrganizationAccount\n    audience: o9 employees (SSO)\n  clients_observed:\n  - name: o9 Platform Wiki\n    client_id: c9fd4e6a-498d-43e9-aedc-3cf50d254308\n    redirect_uri: https://platformwiki.o9solutions.com/index.php/Special:OAuth2Client/callback\n    scope: openid email profile\n  - name: o9 Community\n    client_id: c3efaf96-a57c-48dd-a58d-f07e871b8ba9\n    redirect_uri: https://community.o9solutions.com/auth/oauth2_basic/callback\n\
  \    scope: ''\n  discovery:\n    openid_configuration: not published (404 at /.well-known/openid-configuration and\n      /oauthserver/.well-known/openid-configuration)\n    oauth_authorization_server: not published (404)\ngated_surfaces:\n- name: o9 Platform API reference\n  url: https://guide.o9solutions.com/Resources/ApiDocs\n  observed: redirects to guide.o9solutions.com/oauthserver/authorize\n- name: o9 Reference Model API reference\n  url: https://guide.o9solutions.com/Resources/RefModelApiDoc\n  observed: redirects to guide.o9solutions.com/oauthserver/authorize\n- name: o9 Platform Wiki\n  url: https://platformwiki.o9solutions.com/index.php/Platform_Wiki_-_Table_of_Contents\n  observed: redirects to the OAuth authorize endpoint\nplatform_identity_features:\n  source: https://o9solutions.com/security\n  features:\n  - single sign-on (SSO)\n  - domain claiming\n  - enterprise mobility management (approved-device access)\nx-evidence:\n  fetched: '2026-07-31'\n  urls:\n  - https://guide.o9solutions.com/Resources/ApiDocs\n\
  \  - https://guide.o9solutions.com/Resources/RefModelApiDoc\n  - https://community.o9solutions.com/\n  - https://documents.o9solutions.com/\n  http_status: 200 (pre-authorization page) then 302 to /oauthserver/authorize\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/o9-solutions/refs/heads/main/authentication/o9-solutions-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Supply Chain
- Supply Chain Planning
- Integrated Business Planning
- Demand Planning
- Enterprise Software
- Artificial Intelligence
- Knowledge Graph
- Decision Intelligence
- Retail Planning
- Revenue Growth Management
- Enterprise Resource Planning
---
