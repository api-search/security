---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mlab-sh-batch-triage-api-openapi.yml
  format: yaml
  label: mlab Batch Triage API
  slug: mlab-sh-batch-triage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mlab-sh/openapi/mlab-sh-batch-triage-api-openapi.yml
- filename: mlab-sh-cases-api-openapi.yml
  format: yaml
  label: mlab Cases API
  slug: mlab-sh-cases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mlab-sh/openapi/mlab-sh-cases-api-openapi.yml
- filename: mlab-sh-crypto-api-openapi.yml
  format: yaml
  label: mlab Crypto API
  slug: mlab-sh-crypto-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mlab-sh/openapi/mlab-sh-crypto-api-openapi.yml
- filename: mlab-sh-domain-scan-api-openapi.yml
  format: yaml
  label: mlab Domain Scan API
  slug: mlab-sh-domain-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mlab-sh/openapi/mlab-sh-domain-scan-api-openapi.yml
- filename: mlab-sh-email-analysis-api-openapi.yml
  format: yaml
  label: mlab Email Analysis API
  slug: mlab-sh-email-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mlab-sh/openapi/mlab-sh-email-analysis-api-openapi.yml
- filename: mlab-sh-file-scan-api-openapi.yml
  format: yaml
  label: mlab File Scan API
  slug: mlab-sh-file-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mlab-sh/openapi/mlab-sh-file-scan-api-openapi.yml
- filename: mlab-sh-finding-tags-api-openapi.yml
  format: yaml
  label: mlab Finding Tags API
  slug: mlab-sh-finding-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mlab-sh/openapi/mlab-sh-finding-tags-api-openapi.yml
- filename: mlab-sh-general-api-openapi.yml
  format: yaml
  label: mlab General API
  slug: mlab-sh-general-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mlab-sh/openapi/mlab-sh-general-api-openapi.yml
- filename: mlab-sh-hash-lookup-api-openapi.yml
  format: yaml
  label: mlab Hash Lookup API
  slug: mlab-sh-hash-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mlab-sh/openapi/mlab-sh-hash-lookup-api-openapi.yml
- filename: mlab-sh-ioc-extraction-api-openapi.yml
  format: yaml
  label: mlab IOC Extraction API
  slug: mlab-sh-ioc-extraction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mlab-sh/openapi/mlab-sh-ioc-extraction-api-openapi.yml
- filename: mlab-sh-ip-lookup-api-openapi.yml
  format: yaml
  label: mlab IP Lookup API
  slug: mlab-sh-ip-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mlab-sh/openapi/mlab-sh-ip-lookup-api-openapi.yml
- filename: mlab-sh-limits-api-openapi.yml
  format: yaml
  label: mlab Limits API
  slug: mlab-sh-limits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mlab-sh/openapi/mlab-sh-limits-api-openapi.yml
- filename: mlab-sh-mac-lookup-api-openapi.yml
  format: yaml
  label: mlab MAC Lookup API
  slug: mlab-sh-mac-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mlab-sh/openapi/mlab-sh-mac-lookup-api-openapi.yml
- filename: mlab-sh-phone-analysis-api-openapi.yml
  format: yaml
  label: mlab Phone Analysis API
  slug: mlab-sh-phone-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mlab-sh/openapi/mlab-sh-phone-analysis-api-openapi.yml
- filename: mlab-sh-redkit-api-openapi.yml
  format: yaml
  label: mlab Red Kit API
  slug: mlab-sh-redkit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mlab-sh/openapi/mlab-sh-redkit-api-openapi.yml
- filename: mlab-sh-redkit-flows-api-openapi.yml
  format: yaml
  label: mlab RedKit Flows API
  slug: mlab-sh-redkit-flows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mlab-sh/openapi/mlab-sh-redkit-flows-api-openapi.yml
- filename: mlab-sh-scheduled-scans-api-openapi.yml
  format: yaml
  label: mlab Scheduled Scans API
  slug: mlab-sh-scheduled-scans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mlab-sh/openapi/mlab-sh-scheduled-scans-api-openapi.yml
- filename: mlab-sh-ssl-api-openapi.yml
  format: yaml
  label: mlab SSL API
  slug: mlab-sh-ssl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mlab-sh/openapi/mlab-sh-ssl-api-openapi.yml
- filename: mlab-sh-url-analysis-api-openapi.yml
  format: yaml
  label: mlab URL Analysis API
  slug: mlab-sh-url-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mlab-sh/openapi/mlab-sh-url-analysis-api-openapi.yml
- filename: mlab-sh-vulnerability-monitoring-api-openapi.yml
  format: yaml
  label: mlab Vulnerability Monitoring API
  slug: mlab-sh-vulnerability-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mlab-sh/openapi/mlab-sh-vulnerability-monitoring-api-openapi.yml
- filename: mlab-sh-webhooks-api-openapi.yml
  format: yaml
  label: mlab Webhooks API
  slug: mlab-sh-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mlab-sh/openapi/mlab-sh-webhooks-api-openapi.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: mlab Authentication
name_suffix: Authentication
oauth_flows: []
overview: mlab declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: mlab
provider_slug: mlab-sh
scheme_count: 1
schemes:
- evidence: All API requests require an API key passed in the Authorization header, as Bearer <key> or token <key> .
  header: Authorization
  how_to_obtain: Created in Organization settings → API keys
  location: header
  name: API key
  type: http-bearer
slug: mlab-sh-authentication
source_filename: mlab-sh-authentication.yml
source_heading: Authentication Profile
source_url: https://doc.mlab.sh/docs/mlab.sh/scans/scan-mail-eml
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://doc.mlab.sh/docs/mlab.sh/scans/scan-mail-eml\nsources:\n- https://doc.mlab.sh/docs/mlab.sh/scans/scan-mail-eml\n- https://doc.mlab.sh/docs/mlab.sh/getting-started/api\n- https://doc.mlab.sh/docs/mlab.sh/getting-started/verify-infrastructure\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: All API requests require an API key passed in the Authorization header, as Bearer <key> or token <key> .\n  location: header\n  header: Authorization\n  how_to_obtain: Created in Organization settings → API keys\nnote: No other authentication methods (e.g., OAuth2) are documented on the provided pages.\ndocs: https://doc.mlab.sh/docs/mlab.sh/scans/scan-mail-eml\n"
source_yaml_url: https://artifacts.apis.io/mlab-sh/authentication/mlab-sh-authentication.yml
summary_line: 1 scheme
tags:
- Security
- Threat Intelligence
- IOC
- File Analysis
- Cybersecurity
---
