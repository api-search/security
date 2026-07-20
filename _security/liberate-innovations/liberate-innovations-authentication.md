---
api_key_in: []
api_specs:
- filename: liberate-innovations-orchestration-openapi.yml
  format: yaml
  label: Liberate Orchestration Platform API
  slug: orchestration-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liberate-innovations/refs/heads/main/openapi/liberate-innovations-orchestration-openapi.yml
auth_types: []
description: The Liberate Orchestration Platform API authenticates with a bearer token issued by Liberate. Tokens are scoped per customer and per environment — every customer has both a production and a QA environment, and each has its own unique endpoint URL and token. The exact curl invocation including the correct host is published in the Start Event properties of each workflow inside the Liberate application.
kind: authentication
layout: security
method: searched
name: Liberate Innovations Authentication
name_suffix: Authentication
oauth_flows: []
overview: Liberate Innovations declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Liberate Innovations
provider_slug: liberate-innovations
scheme_count: 0
schemes: []
slug: liberate-innovations-authentication
source_filename: liberate-innovations-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.liberateinc.com/docs/calling-a-workflow\ndocs: https://docs.liberateinc.com/docs/calling-a-workflow\nname: Liberate Orchestration Platform authentication\ndescription: >-\n  The Liberate Orchestration Platform API authenticates with a bearer token issued by Liberate.\n  Tokens are scoped per customer and per environment — every customer has both a production and a\n  QA environment, and each has its own unique endpoint URL and token. The exact curl invocation\n  including the correct host is published in the Start Event properties of each workflow inside the\n  Liberate application.\napis:\n  - name: Liberate Orchestration Platform API\n    spec: openapi/liberate-innovations-orchestration-openapi.yml\n    schemes:\n      - id: bearerAuth\n        type: http\n        scheme: bearer\n        in: header\n        header: Authorization\n        format: 'Authorization: Bearer <token>'\n        description: >-\n     \
  \     A unique bearer token obtained from Liberate. Required on every documented operation\n          (startWorkflow, sendIntermediateEvent).\n        issued_by: Liberate (provisioned, not self-service)\n        self_service: false\n        rotation: not documented publicly\n        environments:\n          - name: production\n            note: Separate token and endpoint URL per customer.\n          - name: qa\n            note: >-\n              Every customer has a QA environment alongside production, with its own endpoint and\n              token. Releases are deployed to QA or production targets.\n        applies_to_operations:\n          - startWorkflow\n          - sendIntermediateEvent\n        evidence: >-\n          'Please note that this request requires a unique bearer token obtained from Liberate.'\n          — https://docs.liberateinc.com/docs/calling-a-workflow\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_key: false\nnotes:\n  - >-\n    OAuth 2 appears in\
  \ the Liberate documentation only as an OUTBOUND connection type — one of the\n    authentication methods (alongside No Authentication, Basic, Bearer Token, API Key, and\n    PostgreSQL) that a Liberate Connection can use when calling an external system from a REST Task.\n    It is not an inbound authentication option for the Liberate API itself. See\n    https://docs.liberateinc.com/docs/connections.\n  - >-\n    Application (console) sign-in is separate from API authentication. Liberate supports SAML\n    single sign-on for the app, brokered through Amazon Cognito; the Google Workspace setup guide\n    documents an ACS URL of the form\n    https://<tenant>.auth.us-west-2.amazoncognito.com/saml2/idpresponse and an Entity ID of the\n    form urn:amazon:cognito:sp:<user-pool-id>. See\n    https://docs.liberateinc.com/docs/google-workspace.\n  - >-\n    No /.well-known/openid-configuration or /.well-known/oauth-authorization-server document is\n    published on any Liberate host. See well-known/liberate-innovations-well-known.yml.\n\
  sso:\n  supported: true\n  protocol: SAML 2.0\n  broker: Amazon Cognito\n  identity_providers_documented:\n    - Google Workspace\n  provisioning: >-\n    Customer downloads IdP metadata and sends it to the Liberate engineering team, who finalize the\n    SSO configuration.\n  docs: https://docs.liberateinc.com/docs/google-workspace\n  evidence: https://www.liberateinc.com/security (FAQ confirms SSO support)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liberate-innovations/refs/heads/main/authentication/liberate-innovations-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Insurance
- InsurTech
- Artificial Intelligence
- Voice AI
- Conversational AI
- Workflow Orchestration
- Claims Automation
- Integration
- Contact Center
---
