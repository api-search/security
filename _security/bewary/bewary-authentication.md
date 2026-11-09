---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bewary-account-api-openapi.yml
  format: yaml
  label: Bewary Account API
  slug: bewary-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-account-api-openapi.yml
- filename: bewary-app-api-openapi.yml
  format: yaml
  label: Bewary App API
  slug: bewary-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-app-api-openapi.yml
- filename: bewary-assess-api-openapi.yml
  format: yaml
  label: Bewary Assess API
  slug: bewary-assess-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-assess-api-openapi.yml
- filename: bewary-backtest-api-openapi.yml
  format: yaml
  label: Bewary Backtest API
  slug: bewary-backtest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-backtest-api-openapi.yml
- filename: bewary-batch-api-openapi.yml
  format: yaml
  label: Bewary Batch API
  slug: bewary-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-batch-api-openapi.yml
- filename: bewary-billing-api-openapi.yml
  format: yaml
  label: Bewary Billing API
  slug: bewary-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-billing-api-openapi.yml
- filename: bewary-bulk-api-openapi.yml
  format: yaml
  label: Bewary Bulk API
  slug: bewary-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-bulk-api-openapi.yml
- filename: bewary-calibration-api-openapi.yml
  format: yaml
  label: Bewary Calibration API
  slug: bewary-calibration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-calibration-api-openapi.yml
- filename: bewary-datasets-api-openapi.yml
  format: yaml
  label: Bewary Datasets API
  slug: bewary-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-datasets-api-openapi.yml
- filename: bewary-directory-api-openapi.yml
  format: yaml
  label: Bewary Directory API
  slug: bewary-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-directory-api-openapi.yml
- filename: bewary-domain-api-openapi.yml
  format: yaml
  label: Bewary Domain API
  slug: bewary-domain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-domain-api-openapi.yml
- filename: bewary-email-api-openapi.yml
  format: yaml
  label: Bewary Email API
  slug: bewary-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-email-api-openapi.yml
- filename: bewary-events-api-openapi.yml
  format: yaml
  label: Bewary Events API
  slug: bewary-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-events-api-openapi.yml
- filename: bewary-iban-api-openapi.yml
  format: yaml
  label: Bewary Iban API
  slug: bewary-iban-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-iban-api-openapi.yml
- filename: bewary-ip-api-openapi.yml
  format: yaml
  label: Bewary Ip API
  slug: bewary-ip-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-ip-api-openapi.yml
- filename: bewary-keys-api-openapi.yml
  format: yaml
  label: Bewary Keys API
  slug: bewary-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-keys-api-openapi.yml
- filename: bewary-payment-handle-api-openapi.yml
  format: yaml
  label: Bewary Payment Handle API
  slug: bewary-payment-handle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-payment-handle-api-openapi.yml
- filename: bewary-phone-api-openapi.yml
  format: yaml
  label: Bewary Phone API
  slug: bewary-phone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-phone-api-openapi.yml
- filename: bewary-shortcode-api-openapi.yml
  format: yaml
  label: Bewary Shortcode API
  slug: bewary-shortcode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-shortcode-api-openapi.yml
- filename: bewary-url-api-openapi.yml
  format: yaml
  label: Bewary URL API
  slug: bewary-url-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-url-api-openapi.yml
- filename: bewary-wallet-api-openapi.yml
  format: yaml
  label: Bewary Wallet API
  slug: bewary-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-wallet-api-openapi.yml
- filename: bewary-watches-api-openapi.yml
  format: yaml
  label: Bewary Watches API
  slug: bewary-watches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-watches-api-openapi.yml
- filename: bewary-webhooks-api-openapi.yml
  format: yaml
  label: Bewary Webhooks API
  slug: bewary-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-webhooks-api-openapi.yml
auth_types: []
description: Authentication schemes as described on Bewary documentation
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bewary Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bewary declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Bewary
provider_slug: bewary
scheme_count: 1
schemes:
- evidence: "Send it in either header: \n```bash\ncurl \"https://api.bewary.app/v1/domain/paypal-login-secure.top\" \\\n  -H \"Authorization: Bearer $BEWARY_API_KEY\"\n```"
  header: Authorization
  how_to_obtain: Create a key at bewary.app/account
  location: header
  name: Authorization
  type: apiKey
slug: bewary-authentication
source_filename: bewary-authentication.yml
source_heading: Authentication Profile
source_url: https://bewary.app/docs/authentication.md
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://bewary.app/docs/authentication.md\nsources:\n- https://bewary.app/docs/authentication.md\n- https://bewary.app/shortcode/44398.json\n- https://bewary.app/docs/authentication\n- https://bewary.app/docs/related\ndescription: Authentication schemes as described on Bewary documentation\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: \"Send it in either header: \\n```bash\\ncurl \\\"https://api.bewary.app/v1/domain/paypal-login-secure.top\\\" \\\\\\n  -H \\\"Authorization:\\\n    \\ Bearer $BEWARY_API_KEY\\\"\\n```\"\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key at bewary.app/account\nnote: No OAuth2, HTTP Bearer, HTTP Basic, JWT, HMAC, mTLS, or other schemes are documented. 1 extracted row(s) were dropped because their quote\n  was not on the page.\ndocs: https://bewary.app/docs/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/bewary/authentication/bewary-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Security
- Fraud Prevention
- MCP
---
