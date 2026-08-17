---
api_key_in: []
api_specs:
- filename: pardot-objects-api-openapi.yml
  format: yaml
  label: Salesforce Marketing Cloud Account Engagement (Pardot) Objects API
  slug: pardot-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pardot/refs/heads/main/openapi/pardot-objects-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Pardot Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Salesforce Marketing Cloud Account Engagement (Pardot) secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Salesforce Marketing Cloud Account Engagement (Pardot)
provider_slug: pardot
scheme_count: 1
schemes:
- description: 'Obtain a Salesforce OAuth 2.0 access token, then send it as `Authorization: Bearer <access_token>` together with `Pardot-Business-Unit-Id: <18-char business unit id>`. The Web Server (authorization code) flow is the documented default; Salesforce supports the full OAuth 2.0 flow set, and the authorization server additionally advertises DPoP signing algorithms and dynamic client registration.'
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    introspectionUrl: https://login.salesforce.com/services/oauth2/introspect
    jwksUri: https://login.salesforce.com/id/keys
    registrationUrl: https://login.salesforce.com/services/oauth2/register
    revocationUrl: https://login.salesforce.com/services/oauth2/revoke
    scopes:
    - pardot_api
    - refresh_token
    - offline_access
    source: https://login.salesforce.com/.well-known/openid-configuration
    tokenUrl: https://login.salesforce.com/services/oauth2/token
    userinfoUrl: https://login.salesforce.com/services/oauth2/userinfo
  name: BearerAuth
  sources:
  - https://developer.salesforce.com/docs/marketing/pardot/guide/authentication.md
  - https://login.salesforce.com/.well-known/openid-configuration
  type: oauth2
slug: pardot-authentication
source_filename: pardot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.salesforce.com/docs/marketing/pardot/guide/authentication.md\ndocs: https://developer.salesforce.com/docs/marketing/pardot/guide/authentication.html\nnote: 'Account Engagement has no authentication of its own — it delegates entirely to Salesforce OAuth 2.0.\n  Two things must be true before any call works: the connected app must carry the pardot_api scope, and the\n  authenticating user must be SSO-enabled (able to reach pi.pardot.com via \"Log In with Salesforce\" or the\n  Account Engagement Lightning App). A bearer token alone is not sufficient: every request also needs the Pardot-Business-Unit-Id\n  header, an 18-character ID beginning \"0Uv\" that a Salesforce admin reads from Setup > Business Unit Setup.\n  The legacy api_key/user_key login is retired.'\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  required_headers:\n  - Authorization\n  - Pardot-Business-Unit-Id\nschemes:\n\
  - name: BearerAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n    revocationUrl: https://login.salesforce.com/services/oauth2/revoke\n    introspectionUrl: https://login.salesforce.com/services/oauth2/introspect\n    registrationUrl: https://login.salesforce.com/services/oauth2/register\n    jwksUri: https://login.salesforce.com/id/keys\n    userinfoUrl: https://login.salesforce.com/services/oauth2/userinfo\n    scopes:\n    - pardot_api\n    - refresh_token\n    - offline_access\n    source: https://login.salesforce.com/.well-known/openid-configuration\n  description: 'Obtain a Salesforce OAuth 2.0 access token, then send it as `Authorization: Bearer <access_token>`\n    together with `Pardot-Business-Unit-Id: <18-char business unit id>`. The Web Server (authorization code)\n    flow is the documented default; Salesforce supports\
  \ the full OAuth 2.0 flow set, and the authorization\n    server additionally advertises DPoP signing algorithms and dynamic client registration.'\n  sources:\n  - https://developer.salesforce.com/docs/marketing/pardot/guide/authentication.md\n  - https://login.salesforce.com/.well-known/openid-configuration\nrequired_headers:\n- name: Authorization\n  value: Bearer <access_token>\n  required: true\n- name: Pardot-Business-Unit-Id\n  value: <18-character Account Engagement Business Unit ID, begins 0Uv>\n  required: true\n  note: Found in Salesforce Setup under \"Business Unit Setup\". Without it the call fails even with a valid\n    token.\nhosts_by_account_type:\n- account_type: Production\n  salesforce_domain: login.salesforce.com\n  api_domain: pi.pardot.com\n- account_type: Account Engagement Developer Org\n  salesforce_domain: login.salesforce.com\n  api_domain: pi.demo.pardot.com\n- account_type: Sandbox\n  salesforce_domain: test.salesforce.com\n  api_domain: pi.demo.pardot.com\n\
  prerequisites:\n- A Salesforce connected app configured for OAuth with the \"pardot_api\" scope selected.\n- The Account Engagement Business Unit ID (18 characters, begins with \"0Uv\").\n- An SSO-enabled Salesforce user who can log in to pi.pardot.com with \"Log In with Salesforce\".\ncaveats:\n- issue: Login IP ranges are not enforced\n  detail: The Account Engagement API does not enforce IP address restrictions configured with the Salesforce\n    \"Enforce login IP ranges on every request\" option. A token that works from one network works from any.\n  source: https://developer.salesforce.com/docs/marketing/pardot/guide/authentication.md\n- issue: Retired credentials\n  detail: The v3-era api_key / user_key login flow (still described by the legacy WADL in schemas/) is retired;\n    OAuth is the only supported path.\n  source: schemas/pardot-schemas.yml\noidc_discovery:\n  url: https://login.salesforce.com/.well-known/openid-configuration\n  http_status: 200\n  file: well-known/pardot-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pardot/refs/heads/main/authentication/pardot-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Marketing Automation
- B2B Marketing
- Lead Generation
- Email Marketing
- Salesforce
- Account Engagement
---
