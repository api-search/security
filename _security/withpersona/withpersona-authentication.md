---
api_key_in: []
api_specs:
- filename: withpersona-accounts-api-openapi.yml
  format: yaml
  label: Persona Accounts API
  slug: withpersona-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-accounts-api-openapi.yml
- filename: withpersona-cases-api-openapi.yml
  format: yaml
  label: Persona Cases API
  slug: withpersona-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-cases-api-openapi.yml
- filename: withpersona-devices-api-openapi.yml
  format: yaml
  label: Persona Devices API
  slug: withpersona-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-devices-api-openapi.yml
- filename: withpersona-documents-api-openapi.yml
  format: yaml
  label: Persona Documents API
  slug: withpersona-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-documents-api-openapi.yml
- filename: withpersona-events-api-openapi.yml
  format: yaml
  label: Persona Events API
  slug: withpersona-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-events-api-openapi.yml
- filename: withpersona-importers-api-openapi.yml
  format: yaml
  label: Persona Importers API
  slug: withpersona-importers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-importers-api-openapi.yml
- filename: withpersona-inquiries-api-openapi.yml
  format: yaml
  label: Persona Inquiries API
  slug: withpersona-inquiries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-inquiries-api-openapi.yml
- filename: withpersona-inquiry-sessions-api-openapi.yml
  format: yaml
  label: Persona Inquiry Sessions API
  slug: withpersona-inquiry-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-inquiry-sessions-api-openapi.yml
- filename: withpersona-reports-api-openapi.yml
  format: yaml
  label: Persona Reports API
  slug: withpersona-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-reports-api-openapi.yml
- filename: withpersona-transactions-api-openapi.yml
  format: yaml
  label: Persona Transactions API
  slug: withpersona-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-transactions-api-openapi.yml
- filename: withpersona-verifications-api-openapi.yml
  format: yaml
  label: Persona Verifications API
  slug: withpersona-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-verifications-api-openapi.yml
- filename: withpersona-webhooks-api-openapi.yml
  format: yaml
  label: Persona Webhooks API
  slug: withpersona-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-webhooks-api-openapi.yml
- filename: withpersona-workflows-api-openapi.yml
  format: yaml
  label: Persona Workflows API
  slug: withpersona-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Withpersona Authentication
name_suffix: Authentication
oauth_flows: []
overview: Persona secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Persona
provider_slug: withpersona
scheme_count: 1
schemes:
- description: Persona API key passed as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/withpersona-openapi.yml
  type: http
slug: withpersona-authentication
source_filename: withpersona-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/withpersona-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Persona API key passed as a Bearer token in the Authorization header.\n  sources:\n  - openapi/withpersona-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/authentication/withpersona-authentication.yml
summary_line: http · 1 scheme
tags:
- Identity
- Identity Verification
- KYC
- KYB
- AML
- Fraud
- Compliance
---
