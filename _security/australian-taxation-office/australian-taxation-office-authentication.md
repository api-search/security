---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: australian-taxation-office-apiinfo-api-openapi.yml
  format: yaml
  label: Australian Taxation Office API Info API
  slug: australian-taxation-office-apiinfo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-apiinfo-api-openapi.yml
- filename: australian-taxation-office-combined-global-and-domestic-group-entity-tax-return-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Combined Global and Domestic Group Entity Tax Return API
  slug: australian-taxation-office-combined-global-and-domestic-group-entity-tax-return-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-combined-global-and-domestic-group-entity-tax-return-api-openapi.yml
- filename: australian-taxation-office-combined-global-and-domestic-minimum-tax-return-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Combined Global and Domestic Minimum Tax Return API
  slug: australian-taxation-office-combined-global-and-domestic-minimum-tax-return-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-combined-global-and-domestic-minimum-tax-return-api-openapi.yml
- filename: australian-taxation-office-get-payee-stapled-super-fund-for-receipt-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Get Payee Stapled Super Fund for Receipt API
  slug: australian-taxation-office-get-payee-stapled-super-fund-for-receipt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-get-payee-stapled-super-fund-for-receipt-api-openapi.yml
- filename: australian-taxation-office-get-payment-reference-number-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Get Payment Reference Number API
  slug: australian-taxation-office-get-payment-reference-number-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-get-payment-reference-number-api-openapi.yml
- filename: australian-taxation-office-gst-property-settlement-date-confirmation-api-openapi.yml
  format: yaml
  label: Australian Taxation Office GST Property Settlement Date Confirmation API
  slug: australian-taxation-office-gst-property-settlement-date-confirmation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-gst-property-settlement-date-confirmation-api-openapi.yml
- filename: australian-taxation-office-gst-property-settlement-withholding-notification-api-openapi.yml
  format: yaml
  label: Australian Taxation Office GST Property Settlement Withholding Notification API
  slug: australian-taxation-office-gst-property-settlement-withholding-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-gst-property-settlement-withholding-notification-api-openapi.yml
- filename: australian-taxation-office-heartbeat-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Heartbeat API
  slug: australian-taxation-office-heartbeat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-heartbeat-api-openapi.yml
- filename: australian-taxation-office-providers-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Providers API
  slug: australian-taxation-office-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-providers-api-openapi.yml
- filename: australian-taxation-office-register-a-new-software-application-instance-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Register a new software application instance API
  slug: australian-taxation-office-register-a-new-software-application-instance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-register-a-new-software-application-instance-api-openapi.yml
- filename: australian-taxation-office-request-stapled-super-fund-for-payee-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Request Stapled Super Fund for Payee API
  slug: australian-taxation-office-request-stapled-super-fund-for-payee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-request-stapled-super-fund-for-payee-api-openapi.yml
- filename: australian-taxation-office-spec-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Spec API
  slug: australian-taxation-office-spec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-spec-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Australian Taxation Office Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Australian Taxation Office secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Australian Taxation Office
provider_slug: australian-taxation-office
scheme_count: 2
schemes:
- description: "API key is assigned when you register to the ATO API Portal.  \n\nSee more details about the registration process in **[Getting started | ATO API Portal](https://apiportal.ato.gov.au/getting-started#toc-how-to-start-using-our-api-portal-services)**."
  in: header
  name: ApiKeyAuth
  parameter: apikey
  sources:
  - openapi/australian-taxation-office-gst-property-settlement-openapi.yml
  type: apiKey
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: '{env}/core2/connect/token'
  name: ScopeAuth
  sources:
  - openapi/australian-taxation-office-gst-property-settlement-openapi.yml
  - openapi/australian-taxation-office-health-check-openapi.yml
  - openapi/australian-taxation-office-oauth-dynamic-client-registration-openapi.yml
  - openapi/australian-taxation-office-stapled-super-fund-openapi.yml
  type: oauth2
slug: australian-taxation-office-authentication
source_filename: australian-taxation-office-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: searched\nsource: https://apiportal.ato.gov.au/client-authentication\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: \"API key is assigned when you register to the ATO API Portal.  \\n\\nSee more details about the registration process in **[Getting started | ATO API Portal](https://apiportal.ato.gov.au/getting-started#toc-how-to-start-using-our-api-portal-services)**.\"\n  sources:\n  - openapi/australian-taxation-office-gst-property-settlement-openapi.yml\n- name: ScopeAuth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: '{env}/core2/connect/token'\n    scopes: 1\n  sources:\n  - openapi/australian-taxation-office-gst-property-settlement-openapi.yml\n  - openapi/australian-taxation-office-health-check-openapi.yml\n  - openapi/australian-taxation-office-oauth-dynamic-client-registration-openapi.yml\n\
  \  - openapi/australian-taxation-office-stapled-super-fund-openapi.yml\ndocs: https://apiportal.ato.gov.au/client-authentication\ntoken_endpoints:\n  production: https://auth.ato.gov.au/core2/connect/token\n  sandbox: https://auth.evte.ato.gov.au/core2/connect/token\ngrants:\n- grant: client_credentials\n  for: directly connected software\n  client_auth: private_key_jwt (client_assertion_type urn:ietf:params:oauth:client-assertion-type:jwt-bearer), RS256, x5c header with the M2M credential signing certificate\n- grant: urn:ietf:params:oauth:grant-type:jwt-bearer (RFC 7523)\n  for: online service providers, with a grant JWT when acting on behalf of a business or intermediary\nrequired_headers:\n- 'Authorization: Bearer <access token>'\n- 'apikey: <consumer key (API key)>'\nclient_registration: Production client ids are issued per software instance via the OAuth Dynamic Client Registration API (registration scope ato.idp.relyingParties.c), after a registration access token\n  is obtained\
  \ from the ATO SSO/IdP.\ncredentials: ATO machine-to-machine (M2M) credential keystore; API keys per team application in the ATO API Portal (separate sandbox and production keys).\nsee_also:\n- https://apiportal.ato.gov.au/api-products/oauth-dynamic-client-registration-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/authentication/australian-taxation-office-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Government
- Taxation
- Superannuation
- Australia
- Digital Service Providers
- Public Sector
---
