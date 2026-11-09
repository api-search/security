---
anonymous_access: false
api_key_in: []
api_specs:
- filename: auravms-com-analytics-export-api-openapi.yml
  format: yaml
  label: AuraVMS Analytics & Export API
  slug: auravms-com-analytics-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auravms-com/openapi/auravms-com-analytics-export-api-openapi.yml
- filename: auravms-com-api-key-management-api-openapi.yml
  format: yaml
  label: AuraVMS API Key Management API
  slug: auravms-com-api-key-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auravms-com/openapi/auravms-com-api-key-management-api-openapi.yml
- filename: auravms-com-attachments-api-openapi.yml
  format: yaml
  label: AuraVMS Attachments API
  slug: auravms-com-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auravms-com/openapi/auravms-com-attachments-api-openapi.yml
- filename: auravms-com-authentication-api-openapi.yml
  format: yaml
  label: AuraVMS Authentication API
  slug: auravms-com-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auravms-com/openapi/auravms-com-authentication-api-openapi.yml
- filename: auravms-com-discovery-api-openapi.yml
  format: yaml
  label: AuraVMS Discovery API
  slug: auravms-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auravms-com/openapi/auravms-com-discovery-api-openapi.yml
- filename: auravms-com-draft-rfqs-api-openapi.yml
  format: yaml
  label: AuraVMS Draft RFQs API
  slug: auravms-com-draft-rfqs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auravms-com/openapi/auravms-com-draft-rfqs-api-openapi.yml
- filename: auravms-com-feedback-api-openapi.yml
  format: yaml
  label: AuraVMS Feedback API
  slug: auravms-com-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auravms-com/openapi/auravms-com-feedback-api-openapi.yml
- filename: auravms-com-reference-data-api-openapi.yml
  format: yaml
  label: AuraVMS Reference Data API
  slug: auravms-com-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auravms-com/openapi/auravms-com-reference-data-api-openapi.yml
- filename: auravms-com-rfq-lifecycle-api-openapi.yml
  format: yaml
  label: AuraVMS RFQ Lifecycle API
  slug: auravms-com-rfq-lifecycle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auravms-com/openapi/auravms-com-rfq-lifecycle-api-openapi.yml
- filename: auravms-com-supplier-management-api-openapi.yml
  format: yaml
  label: AuraVMS Supplier Management API
  slug: auravms-com-supplier-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auravms-com/openapi/auravms-com-supplier-management-api-openapi.yml
auth_types: []
description: AuraVMS authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Auravms Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: AuraVMS declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AuraVMS
provider_slug: auravms-com
scheme_count: 1
schemes:
- evidence: AuraVMS accepts Bearer credentials for protected REST API and MCP operations.
  header: Authorization
  how_to_obtain: Create an API key in the AuraVMS web app under Settings > API Keys (keys begin with avms_) or obtain a JWT access token via the account login endpoint.
  location: header
  name: Bearer
  type: http-bearer
slug: auravms-com-authentication
source_filename: auravms-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.auravms.com/auth.md
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.auravms.com/auth.md\nsources:\n- https://www.auravms.com/auth.md\n- https://www.auravms.com/blogs/vendor-onboarding-checklist-before-first-rfq\n- https://www.auravms.com/blogs/procurement-audit-checklist-internal-controls-compliance-smb-2026\n- https://www.auravms.com/blogs/how-to-simplify-vendor-onboarding-processes\ndescription: AuraVMS authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: AuraVMS accepts Bearer credentials for protected REST API and MCP operations.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the AuraVMS web app under Settings > API Keys (keys begin with avms_) or obtain a JWT access token via the\n    account login endpoint.\ndocs: https://www.auravms.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/auravms-com/authentication/auravms-com-authentication.yml
summary_line: 1 scheme
tags:
- Procurement
- RFQ
- Small Business
- Artificial Intelligence
---
