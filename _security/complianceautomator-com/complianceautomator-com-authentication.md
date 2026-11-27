---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: ComplianceAutomator Authentication
name_suffix: Authentication
oauth_flows: []
overview: ComplianceAutomator declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ComplianceAutomator
provider_slug: complianceautomator-com
scheme_count: 1
schemes:
- applies_to: https://www.complianceautomator.com/api/mcp
  description: 'No authentication documented. Mode: public, read-only, stateless. This endpoint does not expose customer portal, billing, or admin data.'
  name: anonymous
  type: none
slug: complianceautomator-com-authentication
source_filename: complianceautomator-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.complianceautomator.com/mcp\ndocs: https://www.complianceautomator.com/mcp\nsummary: The only programmatic surface is the public MCP endpoint, documented as \"public, read-only, stateless\". The docs list required headers (Content-Type, Accept, MCP-Protocol-Version, Mcp-Method, Mcp-Name) and none of them is a credential; no API key, bearer token or OAuth flow is documented.\nschemes:\n- type: none\n  name: anonymous\n  description: 'No authentication documented. Mode: public, read-only, stateless. This endpoint does not expose customer portal, billing, or admin data.'\n  applies_to: https://www.complianceautomator.com/api/mcp\n"
source_yaml_url: https://artifacts.apis.io/complianceautomator-com/authentication/complianceautomator-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Compliance
- Audit Readiness
- SOC 2
- ISO 27001
- HIPAA
- GDPR
- Governance Risk and Compliance
- Software-as-a-Service
---
