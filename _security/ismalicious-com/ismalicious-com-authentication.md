---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ismalicious-com-action-center-api-openapi.yml
  format: yaml
  label: isMalicious Action Center API
  slug: ismalicious-com-action-center-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ismalicious-com/openapi/ismalicious-com-action-center-api-openapi.yml
- filename: ismalicious-com-alerts-api-openapi.yml
  format: yaml
  label: isMalicious Alerts API
  slug: ismalicious-com-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ismalicious-com/openapi/ismalicious-com-alerts-api-openapi.yml
- filename: ismalicious-com-blocklist-api-openapi.yml
  format: yaml
  label: isMalicious Blocklist API
  slug: ismalicious-com-blocklist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ismalicious-com/openapi/ismalicious-com-blocklist-api-openapi.yml
- filename: ismalicious-com-briefs-api-openapi.yml
  format: yaml
  label: isMalicious Briefs API
  slug: ismalicious-com-briefs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ismalicious-com/openapi/ismalicious-com-briefs-api-openapi.yml
- filename: ismalicious-com-cases-api-openapi.yml
  format: yaml
  label: isMalicious Cases API
  slug: ismalicious-com-cases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ismalicious-com/openapi/ismalicious-com-cases-api-openapi.yml
- filename: ismalicious-com-check-api-openapi.yml
  format: yaml
  label: isMalicious Check API
  slug: ismalicious-com-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ismalicious-com/openapi/ismalicious-com-check-api-openapi.yml
- filename: ismalicious-com-cve-api-openapi.yml
  format: yaml
  label: isMalicious Cve API
  slug: ismalicious-com-cve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ismalicious-com/openapi/ismalicious-com-cve-api-openapi.yml
- filename: ismalicious-com-gate-api-openapi.yml
  format: yaml
  label: isMalicious Gate API
  slug: ismalicious-com-gate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ismalicious-com/openapi/ismalicious-com-gate-api-openapi.yml
- filename: ismalicious-com-mail-api-openapi.yml
  format: yaml
  label: isMalicious Mail API
  slug: ismalicious-com-mail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ismalicious-com/openapi/ismalicious-com-mail-api-openapi.yml
- filename: ismalicious-com-monitoring-api-openapi.yml
  format: yaml
  label: isMalicious Monitoring API
  slug: ismalicious-com-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ismalicious-com/openapi/ismalicious-com-monitoring-api-openapi.yml
- filename: ismalicious-com-platform-api-openapi.yml
  format: yaml
  label: isMalicious Platform API
  slug: ismalicious-com-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ismalicious-com/openapi/ismalicious-com-platform-api-openapi.yml
- filename: ismalicious-com-ransomware-api-openapi.yml
  format: yaml
  label: isMalicious Ransomware API
  slug: ismalicious-com-ransomware-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ismalicious-com/openapi/ismalicious-com-ransomware-api-openapi.yml
- filename: ismalicious-com-search-api-openapi.yml
  format: yaml
  label: isMalicious Search API
  slug: ismalicious-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ismalicious-com/openapi/ismalicious-com-search-api-openapi.yml
- filename: ismalicious-com-stats-api-openapi.yml
  format: yaml
  label: isMalicious Stats API
  slug: ismalicious-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ismalicious-com/openapi/ismalicious-com-stats-api-openapi.yml
- filename: ismalicious-com-submit-api-openapi.yml
  format: yaml
  label: isMalicious Submit API
  slug: ismalicious-com-submit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ismalicious-com/openapi/ismalicious-com-submit-api-openapi.yml
- filename: ismalicious-com-surveillance-api-openapi.yml
  format: yaml
  label: isMalicious Surveillance API
  slug: ismalicious-com-surveillance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ismalicious-com/openapi/ismalicious-com-surveillance-api-openapi.yml
- filename: ismalicious-com-taxii-api-openapi.yml
  format: yaml
  label: isMalicious Taxii API
  slug: ismalicious-com-taxii-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ismalicious-com/openapi/ismalicious-com-taxii-api-openapi.yml
- filename: ismalicious-com-trust-api-openapi.yml
  format: yaml
  label: isMalicious Trust API
  slug: ismalicious-com-trust-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ismalicious-com/openapi/ismalicious-com-trust-api-openapi.yml
- filename: ismalicious-com-webhooks-api-openapi.yml
  format: yaml
  label: isMalicious Webhooks API
  slug: ismalicious-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ismalicious-com/openapi/ismalicious-com-webhooks-api-openapi.yml
auth_types: []
description: Authentication schemes as published on isMalicious pages.
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: isMalicious Authentication
name_suffix: Authentication
oauth_flows: []
overview: isMalicious declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: isMalicious
provider_slug: ismalicious-com
scheme_count: 4
schemes:
- evidence: 'Authentication : with your key pair REST calls to https://api.ismalicious.com accept X-API-KEY (Base64 of apiKey:apiSecret) or HTTP Basic Auth (username=apiKey, password=apiSecret).'
  header: X-API-KEY
  how_to_obtain: Sign up and open Account → API keys to view or rotate credentials; or request a free key via curl -d "email=you@example.com" https://ismalicious.com/api/keys/instant.
  location: header
  name: X-API-KEY
  type: apiKey
- evidence: 'Authentication : with your key pair REST calls to https://api.ismalicious.com accept X-API-KEY (Base64 of apiKey:apiSecret) or HTTP Basic Auth (username=apiKey, password=apiSecret).'
  header: Authorization
  how_to_obtain: Use the same API key pair (apiKey and apiSecret) as username and password.
  location: header
  name: Basic
  type: http-basic
- evidence: 'If none is present, the API returns 401 with "message": "Provide an X-API-KEY header, a Bearer token, HTTP Basic Auth (apiKey:apiSecret), or a valid session cookie".'
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
- evidence: 'If none is present, the API returns 401 with "message": "Provide an X-API-KEY header, a Bearer token, HTTP Basic Auth (apiKey:apiSecret), or a valid session cookie".'
  how_to_obtain: Log in via the web UI to obtain a session cookie.
  location: cookie
  name: Session Cookie
  type: other
slug: ismalicious-com-authentication
source_filename: ismalicious-com-authentication.yml
source_heading: Authentication Profile
source_url: https://ismalicious.com/posts/analyze-dmarc-xml-reports
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://ismalicious.com/posts/analyze-dmarc-xml-reports\nsources:\n- https://ismalicious.com/posts/analyze-dmarc-xml-reports\n- https://ismalicious.com/api-docs/authentication\n- https://ismalicious.com/glossary/api-key\n- https://ismalicious.com/api-docs\ndescription: Authentication schemes as published on isMalicious pages.\nschemes:\n- type: apiKey\n  name: X-API-KEY\n  evidence: 'Authentication : with your key pair REST calls to https://api.ismalicious.com accept X-API-KEY (Base64 of apiKey:apiSecret) or HTTP\n    Basic Auth (username=apiKey, password=apiSecret).'\n  location: header\n  header: X-API-KEY\n  how_to_obtain: Sign up and open Account → API keys to view or rotate credentials; or request a free key via curl -d \"email=you@example.com\"\n    https://ismalicious.com/api/keys/instant.\n- type: http-basic\n  name: Basic\n  evidence: 'Authentication : with your key pair\
  \ REST calls to https://api.ismalicious.com accept X-API-KEY (Base64 of apiKey:apiSecret) or HTTP\n    Basic Auth (username=apiKey, password=apiSecret).'\n  location: header\n  header: Authorization\n  how_to_obtain: Use the same API key pair (apiKey and apiSecret) as username and password.\n- type: http-bearer\n  name: Bearer\n  evidence: 'If none is present, the API returns 401 with \"message\": \"Provide an X-API-KEY header, a Bearer token, HTTP Basic Auth (apiKey:apiSecret),\n    or a valid session cookie\".'\n  location: header\n  header: Authorization\n- type: other\n  name: Session Cookie\n  evidence: 'If none is present, the API returns 401 with \"message\": \"Provide an X-API-KEY header, a Bearer token, HTTP Basic Auth (apiKey:apiSecret),\n    or a valid session cookie\".'\n  location: cookie\n  how_to_obtain: Log in via the web UI to obtain a session cookie.\nnote: No OAuth2 flows are documented on the provided pages.\ndocs: https://ismalicious.com/posts/analyze-dmarc-xml-reports\n"
source_yaml_url: https://artifacts.apis.io/ismalicious-com/authentication/ismalicious-com-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Threat Intelligence
- Cybersecurity
- STIX
- Threat Data
---
