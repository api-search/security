---
anonymous_access: false
api_key_in: []
api_specs:
- filename: licenseground-com-agent-keys-api-openapi.yml
  format: yaml
  label: LicenseGround Agent Keys API
  slug: licenseground-com-agent-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licenseground-com/openapi/licenseground-com-agent-keys-api-openapi.yml
- filename: licenseground-com-agent-topup-api-openapi.yml
  format: yaml
  label: LicenseGround Agent Topup API
  slug: licenseground-com-agent-topup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licenseground-com/openapi/licenseground-com-agent-topup-api-openapi.yml
- filename: licenseground-com-checkout-api-openapi.yml
  format: yaml
  label: LicenseGround Checkout API
  slug: licenseground-com-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licenseground-com/openapi/licenseground-com-checkout-api-openapi.yml
- filename: licenseground-com-compliance-check-api-openapi.yml
  format: yaml
  label: LicenseGround Compliance Check API
  slug: licenseground-com-compliance-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licenseground-com/openapi/licenseground-com-compliance-check-api-openapi.yml
- filename: licenseground-com-federal-api-openapi.yml
  format: yaml
  label: LicenseGround Federal API
  slug: licenseground-com-federal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licenseground-com/openapi/licenseground-com-federal-api-openapi.yml
- filename: licenseground-com-health-api-openapi.yml
  format: yaml
  label: LicenseGround Health API
  slug: licenseground-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licenseground-com/openapi/licenseground-com-health-api-openapi.yml
- filename: licenseground-com-licenseground-api-api-openapi.yml
  format: yaml
  label: LicenseGround LicenseGround API
  slug: licenseground-com-licenseground-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licenseground-com/openapi/licenseground-com-licenseground-api-api-openapi.yml
- filename: licenseground-com-safety-api-openapi.yml
  format: yaml
  label: LicenseGround Safety API
  slug: licenseground-com-safety-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licenseground-com/openapi/licenseground-com-safety-api-openapi.yml
- filename: licenseground-com-search-api-openapi.yml
  format: yaml
  label: LicenseGround Search API
  slug: licenseground-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licenseground-com/openapi/licenseground-com-search-api-openapi.yml
- filename: licenseground-com-stripe-webhook-api-openapi.yml
  format: yaml
  label: LicenseGround Stripe Webhook API
  slug: licenseground-com-stripe-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licenseground-com/openapi/licenseground-com-stripe-webhook-api-openapi.yml
- filename: licenseground-com-verify-api-openapi.yml
  format: yaml
  label: LicenseGround Verify API
  slug: licenseground-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licenseground-com/openapi/licenseground-com-verify-api-openapi.yml
auth_types: []
description: Authentication schemes as published on LicenseGround pages
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: LicenseGround Authentication
name_suffix: Authentication
oauth_flows: []
overview: LicenseGround declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: LicenseGround
provider_slug: licenseground-com
scheme_count: 1
schemes:
- evidence: 'curl -X POST https://licenseground.com/v1/verify \ -H "X-Agent-API-Key: lc_live_sample" \ -H "Content-Type: application/json" \ -d ''{"state": "CA", "license_number": "1048592"}'''
  header: X-Agent-API-Key
  how_to_obtain: Get your free API key by visiting the LicenseGround homepage and clicking 'Get Free Key'.
  location: header
  name: X-Agent-API-Key
  type: apiKey
slug: licenseground-com-authentication
source_filename: licenseground-com-authentication.yml
source_heading: Authentication Profile
source_url: https://licenseground.com/blog/cursor-and-claude-desktop-mcp-contractor-verification-setup
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://licenseground.com/blog/cursor-and-claude-desktop-mcp-contractor-verification-setup\nsources:\n- https://licenseground.com/blog/cursor-and-claude-desktop-mcp-contractor-verification-setup\n- https://licenseground.com/blog/cslb-license-lookup-api-for-ai-agents\ndescription: Authentication schemes as published on LicenseGround pages\nschemes:\n- type: apiKey\n  name: X-Agent-API-Key\n  evidence: 'curl -X POST https://licenseground.com/v1/verify \\ -H \"X-Agent-API-Key: lc_live_sample\" \\ -H \"Content-Type: application/json\" \\ -d\n    ''{\"state\": \"CA\", \"license_number\": \"1048592\"}'''\n  location: header\n  header: X-Agent-API-Key\n  how_to_obtain: Get your free API key by visiting the LicenseGround homepage and clicking 'Get Free Key'.\ndocs: https://licenseground.com/blog/cursor-and-claude-desktop-mcp-contractor-verification-setup\n"
source_yaml_url: https://artifacts.apis.io/licenseground-com/authentication/licenseground-com-authentication.yml
summary_line: 1 scheme
tags:
- Licensing
- Regulatory
- Artificial Intelligence
- Compliance
- Data
---
