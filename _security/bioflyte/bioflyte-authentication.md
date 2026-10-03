---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bioflyte-alert-api-openapi.yml
  format: yaml
  label: BioFlyte Alert API
  slug: bioflyte-alert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioflyte/refs/heads/main/openapi/bioflyte-alert-api-openapi.yml
- filename: bioflyte-client-api-openapi.yml
  format: yaml
  label: BioFlyte Client API
  slug: bioflyte-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioflyte/refs/heads/main/openapi/bioflyte-client-api-openapi.yml
- filename: bioflyte-files-api-openapi.yml
  format: yaml
  label: BioFlyte Files API
  slug: bioflyte-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioflyte/refs/heads/main/openapi/bioflyte-files-api-openapi.yml
- filename: bioflyte-filters-api-openapi.yml
  format: yaml
  label: BioFlyte Filters API
  slug: bioflyte-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioflyte/refs/heads/main/openapi/bioflyte-filters-api-openapi.yml
- filename: bioflyte-locations-api-openapi.yml
  format: yaml
  label: BioFlyte Locations API
  slug: bioflyte-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioflyte/refs/heads/main/openapi/bioflyte-locations-api-openapi.yml
- filename: bioflyte-organization-api-openapi.yml
  format: yaml
  label: BioFlyte Organization API
  slug: bioflyte-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioflyte/refs/heads/main/openapi/bioflyte-organization-api-openapi.yml
- filename: bioflyte-permissions-api-openapi.yml
  format: yaml
  label: BioFlyte Permissions API
  slug: bioflyte-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioflyte/refs/heads/main/openapi/bioflyte-permissions-api-openapi.yml
- filename: bioflyte-requesthelp-api-openapi.yml
  format: yaml
  label: BioFlyte Request Help API
  slug: bioflyte-requesthelp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioflyte/refs/heads/main/openapi/bioflyte-requesthelp-api-openapi.yml
- filename: bioflyte-test-api-openapi.yml
  format: yaml
  label: BioFlyte Test API
  slug: bioflyte-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioflyte/refs/heads/main/openapi/bioflyte-test-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Bioflyte Authentication
name_suffix: Authentication
oauth_flows: []
overview: BioFlyte secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BioFlyte
provider_slug: bioflyte
scheme_count: 1
schemes:
- description: WordPress Application Passwords, advertised by the site at https://www.bioflyte.com/wp-json/ under authentication.application-passwords; authorization endpoint https://www.bioflyte.com/wp-admin/authorize-application.php. Read operations on wp/v2 are anonymous.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/bioflyte-content-openapi.yml
  type: http
slug: bioflyte-authentication
source_filename: bioflyte-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: derived\nsource: openapi/bioflyte-content-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords, advertised by the site at https://www.bioflyte.com/wp-json/\n    under authentication.application-passwords; authorization endpoint https://www.bioflyte.com/wp-admin/authorize-application.php.\n    Read operations on wp/v2 are anonymous.\n  sources:\n  - openapi/bioflyte-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bioflyte/refs/heads/main/authentication/bioflyte-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Biodefense
- Biothreat Detection
- Mass Spectrometry
- Aerosol Monitoring
- Homeland Security
- Critical Infrastructure
- Public Safety
- Sensors
- Hardware
- Artificial Intelligence
- Content
---
