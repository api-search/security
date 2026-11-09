---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods published for Aient
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Aient Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aient declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Aient
provider_slug: aient-ai
scheme_count: 2
schemes:
- evidence: Aient CLI uses customer OAuth for ordinary development work.
  name: customer OAuth
  type: oauth2
- evidence: '`OTEL_EXPORTER_OTLP_HEADERS` makes each export request send `Authorization: Bearer <publishableKey>`.'
  header: Authorization
  location: header
  name: publishable key
  type: http-bearer
slug: aient-ai-authentication
source_filename: aient-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.aient.ai/ai-tools/cli/authentication.md
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.aient.ai/ai-tools/cli/authentication.md\nsources:\n- https://docs.aient.ai/ai-tools/cli/authentication.md\n- https://docs.aient.ai/webhooks/signing.md\n- https://docs.aient.ai/quickstart/opentelemetry.md\n- https://docs.aient.ai/quickstart/server.md\ndescription: Authentication methods published for Aient\nschemes:\n- type: oauth2\n  name: customer OAuth\n  evidence: Aient CLI uses customer OAuth for ordinary development work.\n- type: http-bearer\n  name: publishable key\n  evidence: '`OTEL_EXPORTER_OTLP_HEADERS` makes each export request send `Authorization: Bearer <publishableKey>`.'\n  location: header\n  header: Authorization\ndocs: https://docs.aient.ai/ai-tools/cli/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/aient-ai/authentication/aient-ai-authentication.yml
summary_line: 2 schemes
tags:
- AI SRE
- Automated Fixes
- DevOps
---
