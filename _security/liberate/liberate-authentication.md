---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Liberate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Liberate secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Liberate
provider_slug: liberate
scheme_count: 1
schemes:
- description: A unique bearer token issued by Liberate. The token is scoped to a customer tenant and environment (QA or production); the exact token and endpoint for a given workflow are published in the properties of that workflow's Start Event inside the Liberate console.
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.liberateinc.com/docs/calling-a-workflow
  token_issuance: Issued by Liberate to the customer; not self-service. No public token endpoint is documented.
  type: http
slug: liberate-authentication
source_filename: liberate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.liberateinc.com/docs/calling-a-workflow\ndocs: https://docs.liberateinc.com/docs/calling-a-workflow\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  note: No OpenAPI is published for the Liberate Orchestration Platform API. This profile was read\n    directly from the documented curl invocation for triggering a workflow.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  description: A unique bearer token issued by Liberate. The token is scoped to a customer tenant and\n    environment (QA or production); the exact token and endpoint for a given workflow are published in\n    the properties of that workflow's Start Event inside the Liberate console.\n  token_issuance: Issued by Liberate to the customer; not self-service. No public token endpoint is\n    documented.\n  sources:\n  - https://docs.liberateinc.com/docs/calling-a-workflow\nconsole_sso:\n\
  \  supported: true\n  protocol: SAML 2.0\n  identity_provider_broker: AWS Cognito\n  documented_idps:\n  - Google Workspace\n  acs_url_pattern: https://<tenant>.auth.<region>.amazoncognito.com/saml2/idpresponse\n  entity_id_pattern: urn:amazon:cognito:sp:<user-pool-id>\n  setup: Customer downloads IdP metadata (e.g. GoogleIDPMetadata.xml) and sends it to the Liberate\n    engineering team, who finalize the SSO configuration.\n  docs: https://docs.liberateinc.com/docs/google-workspace\n  note: This is single sign-on for the Liberate web console, not for the workflow-trigger API.\noutbound_connection_auth:\n  description: Auth types Liberate workflows can use when calling OUT to external systems via a\n    Connection. These are consumed by, not exposed by, the Liberate API.\n  docs: https://docs.liberateinc.com/docs/connections\n  types:\n  - none\n  - basic\n  - bearer\n  - apiKey\n  - oauth2\n  - postgresql\n  oauth2_connection_fields:\n  - token_url\n  - client_id\n  - client_secret\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liberate/refs/heads/main/authentication/liberate-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai
- Insurance
- InsurTech
- Voice AI
- AI Agents
- Workflow Orchestration
- Claims Automation
- Low-Code
- Contact Center
---
