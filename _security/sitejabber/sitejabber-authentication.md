---
api_key_in:
- header
- query
api_specs:
- filename: sitejabber-authentication-api-openapi.yml
  format: yaml
  label: SiteJabber Authentication API
  slug: sitejabber-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitejabber/refs/heads/main/openapi/sitejabber-authentication-api-openapi.yml
- filename: sitejabber-business-info-api-openapi.yml
  format: yaml
  label: SiteJabber Business Info API
  slug: sitejabber-business-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitejabber/refs/heads/main/openapi/sitejabber-business-info-api-openapi.yml
- filename: sitejabber-business-questions-api-openapi.yml
  format: yaml
  label: SiteJabber Business Questions API
  slug: sitejabber-business-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitejabber/refs/heads/main/openapi/sitejabber-business-questions-api-openapi.yml
- filename: sitejabber-messages-api-openapi.yml
  format: yaml
  label: SiteJabber Messages API
  slug: sitejabber-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitejabber/refs/heads/main/openapi/sitejabber-messages-api-openapi.yml
- filename: sitejabber-partners-api-openapi.yml
  format: yaml
  label: SiteJabber Partners API
  slug: sitejabber-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitejabber/refs/heads/main/openapi/sitejabber-partners-api-openapi.yml
- filename: sitejabber-privacy-api-openapi.yml
  format: yaml
  label: SiteJabber Privacy API
  slug: sitejabber-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitejabber/refs/heads/main/openapi/sitejabber-privacy-api-openapi.yml
- filename: sitejabber-product-questions-api-openapi.yml
  format: yaml
  label: SiteJabber Product Questions API
  slug: sitejabber-product-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitejabber/refs/heads/main/openapi/sitejabber-product-questions-api-openapi.yml
- filename: sitejabber-product-review-requests-api-openapi.yml
  format: yaml
  label: SiteJabber Product Review Requests API
  slug: sitejabber-product-review-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitejabber/refs/heads/main/openapi/sitejabber-product-review-requests-api-openapi.yml
- filename: sitejabber-product-reviews-api-openapi.yml
  format: yaml
  label: SiteJabber Product Reviews API
  slug: sitejabber-product-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitejabber/refs/heads/main/openapi/sitejabber-product-reviews-api-openapi.yml
- filename: sitejabber-products-api-openapi.yml
  format: yaml
  label: SiteJabber Products API
  slug: sitejabber-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitejabber/refs/heads/main/openapi/sitejabber-products-api-openapi.yml
- filename: sitejabber-resolution-attempts-api-openapi.yml
  format: yaml
  label: SiteJabber Resolution Attempts API
  slug: sitejabber-resolution-attempts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitejabber/refs/heads/main/openapi/sitejabber-resolution-attempts-api-openapi.yml
- filename: sitejabber-review-comments-api-openapi.yml
  format: yaml
  label: SiteJabber Review Comments API
  slug: sitejabber-review-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitejabber/refs/heads/main/openapi/sitejabber-review-comments-api-openapi.yml
- filename: sitejabber-review-requests-api-openapi.yml
  format: yaml
  label: SiteJabber Review Requests API
  slug: sitejabber-review-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitejabber/refs/heads/main/openapi/sitejabber-review-requests-api-openapi.yml
- filename: sitejabber-reviews-api-openapi.yml
  format: yaml
  label: SiteJabber Reviews API
  slug: sitejabber-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitejabber/refs/heads/main/openapi/sitejabber-reviews-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Sitejabber Authentication
name_suffix: Authentication
oauth_flows: []
overview: SiteJabber secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SiteJabber
provider_slug: sitejabber
scheme_count: 2
schemes:
- description: API key issued to the business, passed as a query parameter on every request.
  in: query
  name: client_token
  parameter: client_token
  required: true
  rotation: not documented
  sources:
  - openapi/sitejabber-business-api-openapi.yml
  - https://api.sitejabber.com/
  type: apiKey
- description: User session token returned by POST /login. Typically expires after 6 months; calling login invalidates any previous user token, so concurrent clients sharing one account will evict each other.
  expiry: ~6 months; the login response carries an explicit expire timestamp
  in: header
  name: user_token
  parameter: user_token
  required: true
  required_except:
  - login
  sources:
  - openapi/sitejabber-business-api-openapi.yml
  - https://api.sitejabber.com/
  type: apiKey
slug: sitejabber-authentication
source_filename: sitejabber-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://api.sitejabber.com/ (Authentication section of the published SmartCustomer API reference)\ndocs: https://api.sitejabber.com/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  note: >-\n    Two-part credential, both parts required on every call except login. The client_token API key\n    identifies the business and travels in the QUERY STRING — it will therefore appear in server\n    logs, proxy logs and browser history, which is the notable weakness of this scheme. The\n    user_token is a session token in a request header, obtained by exchanging account credentials\n    at POST /login. There is no OAuth, no OIDC and no scope system: authorization is all-or-nothing\n    per business, enforced server-side (error 308 \"Insufficient permissions\").\nschemes:\n- name: client_token\n  type: apiKey\n  in: query\n  parameter: client_token\n\
  \  description: API key issued to the business, passed as a query parameter on every request.\n  required: true\n  rotation: not documented\n  sources:\n  - openapi/sitejabber-business-api-openapi.yml\n  - https://api.sitejabber.com/\n- name: user_token\n  type: apiKey\n  in: header\n  parameter: user_token\n  description: >-\n    User session token returned by POST /login. Typically expires after 6 months; calling login\n    invalidates any previous user token, so concurrent clients sharing one account will evict each\n    other.\n  required: true\n  required_except:\n  - login\n  expiry: \"~6 months; the login response carries an explicit expire timestamp\"\n  sources:\n  - openapi/sitejabber-business-api-openapi.yml\n  - https://api.sitejabber.com/\nflows:\n- name: token exchange\n  steps:\n  - \"POST https://api.smartcustomer.com/v1/login?client_token={apiKey} with form fields email and password\"\n  - \"Read token and expire from the Login object in the response\"\n  - \"Send the\
  \ returned token as a user_token request header on every subsequent call, alongside the client_token query parameter\"\n  failure_codes:\n  - 101 Client token invalid\n  - 102 Client token access revoked\n  - 201 Email or password invalid\n  - 203 User token missing or invalid\n  - 204 User session is invalid\n  - 207 User token is expired\ncredential_provisioning:\n  url: https://biz.smartcustomer.com/account\n  note: >-\n    The provider's own payload-encryption libraries (packages/) instruct developers to \"get your\n    credentials on biz.sitejabber.com/account\" — now biz.smartcustomer.com. Credentials are issued\n    behind the business login; there is no self-serve public developer signup.\nseparate_encryption_key: >-\n  A distinct CLIENT_ENCRYPTION_KEY (separate from the API client_token) is used by the first-party\n  php-utils/python-utils/java-utils libraries to AES-encrypt a customer payload for the hosted\n  feedback-link flow. It is not an API credential and is not used by\
  \ the REST API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sitejabber/refs/heads/main/authentication/sitejabber-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Reviews
- Consumer Reviews
- Product Reviews
- Reputation Management
- Reviews Management
- E-Commerce
- Trust and Safety
- Google Seller Ratings
- Customer Feedback
- Ratings
- Privacy
---
