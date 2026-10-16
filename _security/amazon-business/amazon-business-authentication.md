---
anonymous_access: false
api_key_in: []
api_specs:
- filename: amazon-business-openapi-generated.yml
  format: yaml
  label: Amazon Business API
  slug: amazon-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-business/refs/heads/main/openapi/_ae-authored/amazon-business-openapi-generated.yml
auth_types: []
description: Amazon Business uses Login with Amazon (LWA) OAuth2 for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Amazon Business Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Business declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Amazon Business
provider_slug: amazon-business
scheme_count: 1
schemes:
- authorize_url: https://www.amazon.com/b2b/abws/oauth?state=100&redirect_uri=
  evidence: Your LWA client identifier and client secret credentials appear. You'll need these credentials to request an LWA access token.
  flows:
  - authorization_code
  how_to_obtain: Create an app in the Solution Provider Portal (SPP) to get the LWA client identifier and client secret.
  name: Login with Amazon
  type: oauth2
slug: amazon-business-authentication
source_filename: amazon-business-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.business.amazon.com/docs/viewing-your-application-information-and-credentials
source_yaml: "generated: '2026-10-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.business.amazon.com/docs/viewing-your-application-information-and-credentials\nsources:\n- https://docs.business.amazon.com/docs/viewing-your-application-information-and-credentials\n- https://docs.business.amazon.com/docs/generate-refresh-token\n- https://docs.business.amazon.com/docs/onboarding-overview\n- https://docs.business.amazon.com/docs/step-1-authorize-your-amazon-business-api-apps\ndescription: Amazon Business uses Login with Amazon (LWA) OAuth2 for authentication.\nschemes:\n- type: oauth2\n  name: Login with Amazon\n  evidence: Your LWA client identifier and client secret credentials appear. You'll need these credentials to request an LWA access token.\n  flows:\n  - authorization_code\n  authorize_url: https://www.amazon.com/b2b/abws/oauth?state=100&redirect_uri=\n  how_to_obtain: Create an app in the Solution Provider Portal (SPP) to get the LWA client\
  \ identifier and client secret.\nnote: The token endpoint is https://api.amazon.com/auth/O2/token as shown in the cURL examples.\ndocs: https://docs.business.amazon.com/docs/viewing-your-application-information-and-credentials\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-business/refs/heads/main/authentication/amazon-business-authentication.yml
summary_line: 1 scheme
tags:
- Company
- B2B
- Procurement
- Marketplace
- BulkPurchasing
---
