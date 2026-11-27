---
anonymous_access: false
api_key_in: []
api_specs:
- filename: contactlint-com-openapi.json
  format: json
  label: ContactLint API
  slug: contactlint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-openapi.json
- filename: contactlint-com-demo-api-openapi.yml
  format: yaml
  label: contactlint-com Demo API
  slug: contactlint-com-demo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-demo-api-openapi.yml
- filename: contactlint-com-demo-preview-api-openapi.yml
  format: yaml
  label: contactlint-com Demo Preview API
  slug: contactlint-com-demo-preview-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-demo-preview-api-openapi.yml
- filename: contactlint-com-demo-preview-rotation-api-openapi.yml
  format: yaml
  label: contactlint-com Demo Preview Rotation API
  slug: contactlint-com-demo-preview-rotation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-demo-preview-rotation-api-openapi.yml
- filename: contactlint-com-domain-api-openapi.yml
  format: yaml
  label: contactlint-com Domain API
  slug: contactlint-com-domain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-domain-api-openapi.yml
- filename: contactlint-com-go-api-openapi.yml
  format: yaml
  label: contactlint-com Go API
  slug: contactlint-com-go-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-go-api-openapi.yml
- filename: contactlint-com-health-api-openapi.yml
  format: yaml
  label: contactlint-com Health API
  slug: contactlint-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-health-api-openapi.yml
- filename: contactlint-com-lookup-api-openapi.yml
  format: yaml
  label: contactlint-com Lookup API
  slug: contactlint-com-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-lookup-api-openapi.yml
- filename: contactlint-com-metrics-api-openapi.yml
  format: yaml
  label: contactlint-com Metrics API
  slug: contactlint-com-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-metrics-api-openapi.yml
- filename: contactlint-com-monitor-api-openapi.yml
  format: yaml
  label: contactlint-com Monitor API
  slug: contactlint-com-monitor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-monitor-api-openapi.yml
- filename: contactlint-com-payment-change-check-api-openapi.yml
  format: yaml
  label: contactlint-com Payment Change Check API
  slug: contactlint-com-payment-change-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-payment-change-check-api-openapi.yml
- filename: contactlint-com-report-api-openapi.yml
  format: yaml
  label: contactlint-com Report API
  slug: contactlint-com-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-report-api-openapi.yml
- filename: contactlint-com-reports-api-openapi.yml
  format: yaml
  label: contactlint-com Reports API
  slug: contactlint-com-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-reports-api-openapi.yml
- filename: contactlint-com-robots-txt-api-openapi.yml
  format: yaml
  label: contactlint-com Robots.txt API
  slug: contactlint-com-robots-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-robots-txt-api-openapi.yml
- filename: contactlint-com-sitemap-xml-api-openapi.yml
  format: yaml
  label: contactlint-com Sitemap.xml API
  slug: contactlint-com-sitemap-xml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-sitemap-xml-api-openapi.yml
auth_types: []
description: ContactLint API uses a secret key sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: contactlint-com Authentication
name_suffix: Authentication
oauth_flows: []
overview: contactlint-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: contactlint-com
provider_slug: contactlint-com
scheme_count: 1
schemes:
- evidence: 'Authorization: "Bearer " + CONTACTLINT_KEY.value()'
  header: Authorization
  how_to_obtain: Get a free secret key at /signup.
  location: header
  name: Bearer
  type: http-bearer
slug: contactlint-com-authentication
source_filename: contactlint-com-authentication.yml
source_heading: Authentication Profile
source_url: https://contactlint.com/integrations/firebase-authentication
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://contactlint.com/integrations/firebase-authentication\nsources:\n- https://contactlint.com/integrations/firebase-authentication\n- https://contactlint.com/integrations\n- https://contactlint.com/integrations/supabase\ndescription: ContactLint API uses a secret key sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authorization: \"Bearer \" + CONTACTLINT_KEY.value()'\n  location: header\n  header: Authorization\n  how_to_obtain: Get a free secret key at /signup.\nnote: No other authentication schemes (apiKey, oauth2, etc.) are documented on the pages.\ndocs: https://contactlint.com/integrations/firebase-authentication\n"
source_yaml_url: https://artifacts.apis.io/contactlint-com/authentication/contactlint-com-authentication.yml
summary_line: 1 scheme
tags:
- Email Verification
- Phone Validation
- MCP
- Developer Tools
- Company
---
