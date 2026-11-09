---
anonymous_access: false
api_key_in: []
api_specs:
- filename: feedback-tools-openapi-generated.yml
  format: yaml
  label: Feedback.tools API
  slug: feedback-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedback-tools/openapi/_ae-authored/feedback-tools-openapi-generated.yml
auth_types: []
description: Webhook request authentication using a secret HMAC signature.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Feedback Tools Authentication
name_suffix: Authentication
oauth_flows: []
overview: Feedback.tools declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Feedback.tools
provider_slug: feedback-tools
scheme_count: 1
schemes:
- evidence: Every webhook request sent by feedback.tools includes an `X-Webhook-Signature` header so you can verify the request came from feedback.tools and was not tampered with.
  header: X-Webhook-Signature
  how_to_obtain: The secret is generated automatically when you create a webhook integration and can be viewed or rotated via the integration settings.
  location: header
  name: Webhook secret
  type: apiKey
slug: feedback-tools-authentication
source_filename: feedback-tools-authentication.yml
source_heading: Authentication Profile
source_url: https://feedback.tools/docs/integrations/webhook-signing.md
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://feedback.tools/docs/integrations/webhook-signing.md\nsources:\n- https://feedback.tools/docs/integrations/webhook-signing.md\n- https://feedback.tools/docs/integrations/webhook-signing\n- https://feedback.tools/react-feedback-surveys/docs.md\n- https://feedback.tools/docs/sdk\ndescription: Webhook request authentication using a secret HMAC signature.\nschemes:\n- type: apiKey\n  name: Webhook secret\n  evidence: Every webhook request sent by feedback.tools includes an `X-Webhook-Signature` header so you can verify the request came from feedback.tools\n    and was not tampered with.\n  location: header\n  header: X-Webhook-Signature\n  how_to_obtain: The secret is generated automatically when you create a webhook integration and can be viewed or rotated via the integration\n    settings.\ndocs: https://feedback.tools/docs/integrations/webhook-signing.md\n"
source_yaml_url: https://artifacts.apis.io/feedback-tools/authentication/feedback-tools-authentication.yml
summary_line: 1 scheme
tags:
- Feedback
- Analytics
- Customer
- AI
- SaaS
---
