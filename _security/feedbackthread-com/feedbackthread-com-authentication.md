---
anonymous_access: false
api_key_in: []
api_specs:
- filename: feedbackthread-com-openapi-generated.yml
  format: yaml
  label: FeedbackThread API
  slug: feedbackthread-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedbackthread-com/openapi/_ae-authored/feedbackthread-com-openapi-generated.yml
auth_types: []
description: Authentication for the FeedbackThread MCP endpoint.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: FeedbackThread Authentication
name_suffix: Authentication
oauth_flows: []
overview: FeedbackThread declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FeedbackThread
provider_slug: feedbackthread-com
scheme_count: 1
schemes:
- evidence: Streamable HTTP, authenticated with a bearer token.
  header: Authorization
  how_to_obtain: 'Create a token From the dashboard, open MCP access and create a token:'
  location: header
  name: Bearer token
  type: http-bearer
slug: feedbackthread-com-authentication
source_filename: feedbackthread-com-authentication.yml
source_heading: Authentication Profile
source_url: https://feedbackthread.com/docs/mcp
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://feedbackthread.com/docs/mcp\nsources:\n- https://feedbackthread.com/docs/mcp\ndescription: Authentication for the FeedbackThread MCP endpoint.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: Streamable HTTP, authenticated with a bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: 'Create a token From the dashboard, open MCP access and create a token:'\nnote: No OAuth flows or other authentication types are documented on the page.\ndocs: https://feedbackthread.com/docs/mcp\n"
source_yaml_url: https://artifacts.apis.io/feedbackthread-com/authentication/feedbackthread-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Feedback
- Reviews
- IndieDevelopers
- Software-as-a-Service
---
