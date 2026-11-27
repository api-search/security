---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for AgentReady API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: AgentReady (Ingenious AI) Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentReady (Ingenious AI) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AgentReady (Ingenious AI)
provider_slug: agentready-getingeniousai-com
scheme_count: 1
schemes:
- evidence: 'A bearer credential for AgentReady''s programmatic interface: created in the app, prefixed ar_key_ for recognisability, stored only as a SHA-256 hash, and shown in full exactly once at creation.'
  header: Authorization
  how_to_obtain: Create a key in the app; the full secret is displayed a single time.
  location: header
  name: API Key
  type: http-bearer
slug: agentready-getingeniousai-com-authentication
source_filename: agentready-getingeniousai-com-authentication.yml
source_heading: Authentication Profile
source_url: https://agentready.getingeniousai.com/guides/api-keys-for-your-store-scans
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://agentready.getingeniousai.com/guides/api-keys-for-your-store-scans\nsources:\n- https://agentready.getingeniousai.com/guides/api-keys-for-your-store-scans\n- https://agentready.getingeniousai.com/guides/agency-onboarding-a-client-store\ndescription: Authentication schemes for AgentReady API\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'A bearer credential for AgentReady''s programmatic interface: created in the app, prefixed ar_key_ for recognisability, stored only\n    as a SHA-256 hash, and shown in full exactly once at creation.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the app; the full secret is displayed a single time.\ndocs: https://agentready.getingeniousai.com/guides/api-keys-for-your-store-scans\n"
source_yaml_url: https://artifacts.apis.io/agentready-getingeniousai-com/authentication/agentready-getingeniousai-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- E-Commerce
- Store
- Catalog
---
