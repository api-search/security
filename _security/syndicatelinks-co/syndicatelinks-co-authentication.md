---
anonymous_access: false
api_key_in: []
api_specs:
- filename: syndicatelinks-co-openapi-generated.yml
  format: yaml
  label: Syndicate Links API
  slug: syndicatelinks-co-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/syndicatelinks-co/openapi/_ae-authored/syndicatelinks-co-openapi-generated.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Syndicate Links Authentication
name_suffix: Authentication
oauth_flows: []
overview: Syndicate Links declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Syndicate Links
provider_slug: syndicatelinks-co
scheme_count: 1
schemes:
- evidence: 'Header: Authorization: Bearer aff_agent_...'
  header: Authorization
  how_to_obtain: Request an aff_agent_ key via POST /affiliate/register with type=agent.
  location: header
  name: Bearer
  type: http-bearer
slug: syndicatelinks-co-authentication
source_filename: syndicatelinks-co-authentication.yml
source_heading: Authentication Profile
source_url: https://syndicatelinks.co/docs/agent-integration/
source_yaml: "generated: '2026-11-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://syndicatelinks.co/docs/agent-integration/\nsources:\n- https://syndicatelinks.co/docs/agent-integration/\n- https://syndicatelinks.co/docs/signed-attribution-tokens/\n- https://syndicatelinks.co/docs/agent-attribution-spec/\n- https://syndicatelinks.co/docs/getting-started/\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Header: Authorization: Bearer aff_agent_...'\n  location: header\n  header: Authorization\n  how_to_obtain: Request an aff_agent_ key via POST /affiliate/register with type=agent.\nnote: Other key types (mk_live_, ak_live_) exist but are not used for agent authentication.\ndocs: https://syndicatelinks.co/docs/agent-integration/\n"
source_yaml_url: https://artifacts.apis.io/syndicatelinks-co/authentication/syndicatelinks-co-authentication.yml
summary_line: 1 scheme
tags:
- Affiliate
- API
- Payments
- AI
- Attribution
- Commerce
---
