---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dealogic-admin-api-openapi.yml
  format: yaml
  label: Dealogic Admin API
  slug: dealogic-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-admin-api-openapi.yml
- filename: dealogic-data-api-openapi.yml
  format: yaml
  label: Dealogic Data API
  slug: dealogic-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-data-api-openapi.yml
- filename: dealogic-dcmdeal-api-openapi.yml
  format: yaml
  label: Dealogic Dcm Deal API
  slug: dealogic-dcmdeal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-dcmdeal-api-openapi.yml
- filename: dealogic-entity-navigation-api-openapi.yml
  format: yaml
  label: Dealogic Entity Navigation API
  slug: dealogic-entity-navigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-entity-navigation-api-openapi.yml
- filename: dealogic-levfinmarketupdate-api-openapi.yml
  format: yaml
  label: Dealogic Levfin Market Update API
  slug: dealogic-levfinmarketupdate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-levfinmarketupdate-api-openapi.yml
- filename: dealogic-loandeal-api-openapi.yml
  format: yaml
  label: Dealogic Loan Deal API
  slug: dealogic-loandeal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-loandeal-api-openapi.yml
- filename: dealogic-organizationspacprofile-api-openapi.yml
  format: yaml
  label: Dealogic Organization Spac Profile API
  slug: dealogic-organizationspacprofile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-organizationspacprofile-api-openapi.yml
- filename: dealogic-related-entities-api-openapi.yml
  format: yaml
  label: Dealogic Related Entities API
  slug: dealogic-related-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-related-entities-api-openapi.yml
- filename: dealogic-reportdata-api-openapi.yml
  format: yaml
  label: Dealogic Report Data API
  slug: dealogic-reportdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-reportdata-api-openapi.yml
- filename: dealogic-root-entity-api-openapi.yml
  format: yaml
  label: Dealogic Root Entity API
  slug: dealogic-root-entity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-root-entity-api-openapi.yml
- filename: dealogic-spac-admin-api-openapi.yml
  format: yaml
  label: Dealogic Spac Admin API
  slug: dealogic-spac-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-spac-admin-api-openapi.yml
- filename: dealogic-spac-reader-api-openapi.yml
  format: yaml
  label: Dealogic Spac Reader API
  slug: dealogic-spac-reader-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-spac-reader-api-openapi.yml
- filename: dealogic-spac-writer-api-openapi.yml
  format: yaml
  label: Dealogic Spac Writer API
  slug: dealogic-spac-writer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-spac-writer-api-openapi.yml
- filename: dealogic-test-api-openapi.yml
  format: yaml
  label: Dealogic Test API
  slug: dealogic-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-test-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dealogic Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Dealogic secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Dealogic
provider_slug: dealogic
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://login.dealogic.com/as/authorization.oauth2
    flow: implicit
    note: The scopes map is EMPTY in every published spec. The scopes the authorization server actually advertises are in scopes/dealogic-scopes.yml, read from the OIDC discovery document.
    scopes_declared_in_spec: 0
    tokenUrl: https://login.dealogic.com/as/token.oauth2
  header: Authorization
  in: header
  name: oauth2
  prefix: Bearer
  sources:
  - openapi/dealogic-analytics-spac-v2-openapi.json
  - openapi/dealogic-analytics-spac-v1-openapi.json
  - openapi/dealogic-analytics-bank-openapi.json
  - openapi/dealogic-analytics-company-openapi.json
  - openapi/dealogic-analytics-sponsor-openapi.json
  - openapi/dealogic-reporting-openapi.json
  - openapi/dealogic-cortex-reporting-openapi.json
  - openapi/dealogic-iona-profiles-openapi.json
  type: oauth2
slug: dealogic-authentication
source_filename: dealogic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://login.dealogic.com/.well-known/openid-configuration (HTTP 200, fetched 2026-09-05) and\n  the oauth2 securityScheme declared in all eight harvested OpenAPI documents\ndocs: https://iongroup.com/analytics/data-portal/apis-data-feeds/\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - implicit\n  note: 'Every Dealogic HTTP API harvested declares exactly one securityScheme: OAuth 2.0 implicit against\n    the shared Dealogic identity provider at login.dealogic.com. There is no API-key path. Unauthenticated\n    calls return 401 with an empty body (probed 2026-09-05 against https://spac.analytics.dealogic.com/odata/SpacEntry).'\nidentity_provider:\n  issuer: https://login.dealogic.com\n  product: PingFederate\n  evidence:\n  - https://login.dealogic.com/pf/JWKS returns the JWKS (HTTP 200)\n  - userinfo_endpoint is https://login.dealogic.com/idp/userinfo.openid\n  - grant_types_supported includes urn:pingidentity.com:oauth2:grant_type:validate_bearer\n\
  \  discovery:\n  - url: https://login.dealogic.com/.well-known/openid-configuration\n    status: 200\n    file: well-known/dealogic-login-dealogic-com-openid-configuration.json\n  - url: https://login.dealogic.com/.well-known/oauth-authorization-server\n    status: 200\n    file: well-known/dealogic-login-dealogic-com-oauth-authorization-server.json\nschemes:\n- name: oauth2\n  type: oauth2\n  in: header\n  header: Authorization\n  prefix: Bearer\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.dealogic.com/as/authorization.oauth2\n    tokenUrl: https://login.dealogic.com/as/token.oauth2\n    scopes_declared_in_spec: 0\n    note: The scopes map is EMPTY in every published spec. The scopes the authorization server actually\n      advertises are in scopes/dealogic-scopes.yml, read from the OIDC discovery document.\n  sources:\n  - openapi/dealogic-analytics-spac-v2-openapi.json\n  - openapi/dealogic-analytics-spac-v1-openapi.json\n  - openapi/dealogic-analytics-bank-openapi.json\n\
  \  - openapi/dealogic-analytics-company-openapi.json\n  - openapi/dealogic-analytics-sponsor-openapi.json\n  - openapi/dealogic-reporting-openapi.json\n  - openapi/dealogic-cortex-reporting-openapi.json\n  - openapi/dealogic-iona-profiles-openapi.json\nendpoints:\n  authorization: https://login.dealogic.com/as/authorization.oauth2\n  token: https://login.dealogic.com/as/token.oauth2\n  userinfo: https://login.dealogic.com/idp/userinfo.openid\n  jwks: https://login.dealogic.com/pf/JWKS\n  introspection: https://login.dealogic.com/as/introspect.oauth2\n  revocation: https://login.dealogic.com/as/revoke_token.oauth2\n  end_session: https://login.dealogic.com/idp/init_logout.openid\ngrant_types_supported:\n- implicit\n- authorization_code\n- refresh_token\n- password\n- client_credentials\n- urn:pingidentity.com:oauth2:grant_type:validate_bearer\n- urn:ietf:params:oauth:grant-type:jwt-bearer\n- urn:ietf:params:oauth:grant-type:saml2-bearer\n- urn:ietf:params:oauth:grant-type:device_code\n\
  - urn:ietf:params:oauth:grant-type:token-exchange\n- urn:openid:params:grant-type:ciba\ntoken_endpoint_auth_methods_supported:\n- client_secret_basic\n- client_secret_post\n- client_secret_jwt\n- private_key_jwt\n- tls_client_auth\n- none\npkce:\n  supported: true\n  code_challenge_methods:\n  - plain\n  - S256\nclient_ids_published_in_swagger_ui:\n- client_id: Dealogic.Analytics.Spac\n  ui: https://spac.analytics.dealogic.com/index.html\n- client_id: Dealogic.Analytics\n  ui: https://bank.analytics.dealogic.com/index.html\n- client_id: Reporting.API\n  ui: https://api.reporting.dealogic.com/index.html\nonboarding:\n  self_service: false\n  note: No self-service signup or key issuance. OAuth clients are provisioned to licensed customers; access\n    starts with the ION Analytics request-information form.\n  url: https://iongroup.com/analytics/data-portal/request-info/\nfeed_authentication:\n  api: Dealogic Primary Market Deals & Entities Feed\n  type: username/password on the Dealogic\
  \ secure FTP server\n  source: https://iongroup.com/analytics/data-portal/apis-data-feeds/dealogic-origination-data-feed/authentication-and-authorization/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/authentication/dealogic-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Analytics
- Capital Markets
- Compliance
- Deal Management
- Debt Capital Markets
- Equity Capital Markets
- Finance
- Financial Data
- Investment Banking
- League Tables
- M&A
- OData
- Private Equity
- Reporting
- SPAC
- Syndicated Loans
---
