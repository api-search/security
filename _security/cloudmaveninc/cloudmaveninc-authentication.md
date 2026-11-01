---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cloudmaveninc-openapi-generated.yml
  format: yaml
  label: Cloud Maven API
  slug: cloudmaveninc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudmaveninc/openapi/_ae-authored/cloudmaveninc-openapi-generated.yml
auth_types: []
description: Authentication schemes for Cloud Maven connectors as documented.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cloudmaveninc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloud Maven declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Cloud Maven
provider_slug: cloudmaveninc
scheme_count: 1
schemes:
- evidence: Updates QuickBooks OAuth credentials and State URL for a specified QuickBooks Credential record.
  how_to_obtain: Provide clientId, clientSecret, and stateURL via the AdminServices.updateQBCredentials method.
  name: QuickBooks OAuth
  token_url: https://oauth.platform.intuit.com/oauth2/v1/tokens/bearer
  type: oauth2
slug: cloudmaveninc-authentication
source_filename: cloudmaveninc-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.cloudmaveninc.com/quickbooks-connector/api-guide/quickbooks-credentials-update-snippets.md
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.cloudmaveninc.com/quickbooks-connector/api-guide/quickbooks-credentials-update-snippets.md\nsources:\n- https://docs.cloudmaveninc.com/quickbooks-connector/api-guide/quickbooks-credentials-update-snippets.md\n- https://docs.cloudmaveninc.com/bank-connect/admin-guide/set-up-plaid-credentials-features-via-script.md\n- https://docs.cloudmaveninc.com/docgen-esign/user-guide/document-signing-certificate.md\n- https://docs.cloudmaveninc.com/thomson-reuters-clear/admin-guide/how-to-setup-clear-credentials.md\ndescription: Authentication schemes for Cloud Maven connectors as documented.\nschemes:\n- type: oauth2\n  name: QuickBooks OAuth\n  evidence: Updates QuickBooks OAuth credentials and State URL for a specified QuickBooks Credential record.\n  token_url: https://oauth.platform.intuit.com/oauth2/v1/tokens/bearer\n  how_to_obtain: Provide clientId, clientSecret, and stateURL\
  \ via the AdminServices.updateQBCredentials method.\ndocs: https://docs.cloudmaveninc.com/quickbooks-connector/api-guide/quickbooks-credentials-update-snippets.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/cloudmaveninc/authentication/cloudmaveninc-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Automation
- Salesforce
- FinTech
- Lending
---
