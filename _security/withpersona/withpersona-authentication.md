---
api_key_in: []
api_specs:
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Inquiries API
  slug: persona-inquiries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Inquiry Sessions API
  slug: persona-inquiry-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Accounts API
  slug: persona-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Verifications API
  slug: persona-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Reports API
  slug: persona-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Cases API
  slug: persona-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Transactions API
  slug: persona-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Devices API
  slug: persona-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Documents API
  slug: persona-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Webhooks API
  slug: persona-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Events API
  slug: persona-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Importers API
  slug: persona-importers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Workflows API
  slug: persona-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
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
