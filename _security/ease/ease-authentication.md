---
api_key_in: []
api_specs:
- filename: ease-content-openapi.yml
  format: yaml
  label: Ease Content & Marketplace API
  slug: ease-content-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ease/refs/heads/main/openapi/ease-content-openapi.yml
- filename: ease-status-openapi.yml
  format: yaml
  label: Ease Status API
  slug: ease-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ease/refs/heads/main/openapi/ease-status-openapi.yml
auth_types:
- none
- http
description: ''
kind: authentication
layout: security
method: searched
name: Ease Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ease secures its APIs with none and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ease
provider_slug: ease
scheme_count: 2
schemes:
- applies_to:
  - openapi/ease-content-openapi.yml
  - openapi/ease-status-openapi.yml
  name: anonymous
  note: Every published operation returns 200 with no credentials. Verified live 2026-07-25.
  type: none
- applies_to_operations: none of the published operations
  description: WordPress Application Passwords, advertised by the site itself in the "authentication" block of https://www.ease.com/wp-json/ (authorization endpoint https://www.ease.com/wp-admin/authorize-application.php). Site administration only; not a developer program, and not required by any operation in this repo.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/ease-content-openapi.yml
  type: http
slug: ease-authentication
source_filename: ease-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  openapi/ease-content-openapi.yml , openapi/ease-status-openapi.yml , the authentication block of\n  https://www.ease.com/wp-json/ , https://www.ease.com/product/security/sso/ , and live probes of\n  every Ease host on 2026-07-25\ndocs: https://www.ease.com/product/security/sso/\nsummary:\n  types:\n  - none\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  public_read: true\n  developer_credentials_available: false\nstatement: >-\n  Ease issues no developer credentials. Both of its public machine-readable surfaces - the\n  www.ease.com WordPress content API and the status.ease.com Statuspage v2 API - are fully\n  anonymous for every operation captured in this repo. The only authentication scheme advertised\n  anywhere is WordPress Application Passwords (HTTP Basic), which guards the site-administration\n  routes that are deliberately excluded from openapi/ease-content-openapi.yml. There is no OAuth\n  2.0, no OpenID\
  \ Connect discovery, no API-key programme and no self-serve signup for any Ease\n  API. Access to the real integration surfaces - EaseConnect (X12 834), EaseConnect+ direct\n  carrier connections - is negotiated privately and administered behind the customer login.\nschemes:\n- name: anonymous\n  type: none\n  applies_to:\n  - openapi/ease-content-openapi.yml\n  - openapi/ease-status-openapi.yml\n  note: Every published operation returns 200 with no credentials. Verified live 2026-07-25.\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: >-\n    WordPress Application Passwords, advertised by the site itself in the \"authentication\" block\n    of https://www.ease.com/wp-json/ (authorization endpoint\n    https://www.ease.com/wp-admin/authorize-application.php). Site administration only; not a\n    developer program, and not required by any operation in this repo.\n  sources:\n  - openapi/ease-content-openapi.yml\n  applies_to_operations: none of the published operations\n\
  negative_findings:\n  oauth2: 'No /.well-known/oauth-authorization-server on www.ease.com, secure.ease.com or api.ease.com (all 404).'\n  openid_connect: 'No /.well-known/openid-configuration on any Ease host (all 404).'\n  api_keys: No key issuance, key management or key documentation anywhere on ease.com.\n  mutual_tls: Not documented.\n  scopes: 'No OAuth scope surface exists; scopes/ is deliberately absent - scopes are OAuth-only.'\napplication_authentication:\n  scope: The Ease product at secure.ease.com, not an API\n  factors:\n  - username and password\n  - mandatory two-factor authentication for all users\n  federation:\n    protocol: SAML 2.0\n    provider: Okta\n    availability: Enterprise pricing package\n    docs: https://www.ease.com/product/security/sso/\n  note: >-\n    developer.ease.com, developers.ease.com, api.ease.com and docs.ease.com all resolve through\n    wildcard DNS to this sign-in page. A 200 from those hostnames is a login wall, not an API.\npartner_authentication:\n\
  \  easeconnect:\n    mechanism: ANSI X12 EDI 834 file exchange, mapped per carrier inside the Ease application\n    access: customer/broker login\n  easeconnect_plus:\n    mechanism: privately negotiated direct data connection between Ease and a carrier\n    access: >-\n      arranged by Ease implementation analysts; includes an undocumented Evidence of Insurability\n      API and Member Benefits API in the Principal integration\n  partner_portal:\n    mechanism: scheduled reports downloaded from the portal or delivered over SFTP\n    access: partner login\ncross_links:\n  conventions: conventions/ease-conventions.yml\n  conformance: conformance/ease-conformance.yml\n  domain_security: security/ease-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ease/refs/heads/main/authentication/ease-authentication.yml
summary_line: none/http · 2 schemes
tags:
- Insurance
- United States
- Employee Benefits
- Benefits Administration
- Group Benefits
- Health Insurance
- Insurtech
- Brokers
- Enrollment
- EDI
- Payroll
- Human Resources
- Marketplace
- Status
---
