---
anonymous_access: false
api_key_in: []
api_specs:
- filename: amazon-payment-services-openapi-generated.yml
  format: yaml
  label: Amazon Payment Services API
  slug: amazon-payment-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-payment-services/openapi/_ae-authored/amazon-payment-services-openapi-generated.yml
auth_types: []
description: Authentication for Amazon Payment Services APIs is performed by including the merchant's access_code, merchant_identifier, and a SHA‑256 signature in the JSON request body.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Amazon Payment Services Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Payment Services declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Amazon Payment Services
provider_slug: amazon-payment-services
scheme_count: 1
schemes:
- evidence: 'access_code   Alphanumeric Max: 20 Required Merchant access code obtained from Amazon Payment Services dashboard under Integration Settings.'
  how_to_obtain: Obtain the access_code, merchant_identifier, SHA request phrase, and SHA response phrase from the Amazon Payment Services merchant dashboard under Integration Settings → Security Settings.
  location: body
  name: Amazon Payment Services API credentials
  type: other
slug: amazon-payment-services-authentication
source_filename: amazon-payment-services-authentication.yml
source_heading: Authentication Profile
source_url: https://paymentservices.amazon.com/docs/api/managing-payments/void-auth
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://paymentservices.amazon.com/docs/api/managing-payments/void-auth\nsources:\n- https://paymentservices.amazon.com/docs/api/managing-payments/void-auth\n- https://docs.aws.amazon.com/IAM/latest/UserGuide/security-creds.html?icmpid=docs_homepage_genref\n- https://paymentservices.amazon.com/docs/getting-started\n- https://paymentservices.amazon.com/docs/accepting-payments/hosted-checkout/overview\ndescription: Authentication for Amazon Payment Services APIs is performed by including the merchant's access_code, merchant_identifier, and a\n  SHA‑256 signature in the JSON request body.\nschemes:\n- type: other\n  name: Amazon Payment Services API credentials\n  evidence: 'access_code   Alphanumeric Max: 20 Required Merchant access code obtained from Amazon Payment Services dashboard under Integration\n    Settings.'\n  location: body\n  how_to_obtain: Obtain the access_code, merchant_identifier,\
  \ SHA request phrase, and SHA response phrase from the Amazon Payment Services merchant\n    dashboard under Integration Settings → Security Settings.\nnote: No OAuth2, API key in header, or other authentication mechanisms are documented on the provided pages.\ndocs: https://paymentservices.amazon.com/docs/api/managing-payments/void-auth\n"
source_yaml_url: https://artifacts.apis.io/amazon-payment-services/authentication/amazon-payment-services-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Payments
- FinTech
- API
- E-commerce
- PaymentsGateway
---
