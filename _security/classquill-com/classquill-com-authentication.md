---
anonymous_access: false
api_key_in: []
api_specs:
- filename: classquill-com-billing-api-openapi.yml
  format: yaml
  label: ClassQuill Billing API
  slug: classquill-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classquill-com/openapi/classquill-com-billing-api-openapi.yml
- filename: classquill-com-blog-api-openapi.yml
  format: yaml
  label: ClassQuill Blog API
  slug: classquill-com-blog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classquill-com/openapi/classquill-com-blog-api-openapi.yml
- filename: classquill-com-bookings-api-openapi.yml
  format: yaml
  label: ClassQuill Bookings API
  slug: classquill-com-bookings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classquill-com/openapi/classquill-com-bookings-api-openapi.yml
- filename: classquill-com-coursework-api-openapi.yml
  format: yaml
  label: ClassQuill Coursework API
  slug: classquill-com-coursework-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classquill-com/openapi/classquill-com-coursework-api-openapi.yml
- filename: classquill-com-curriculum-api-openapi.yml
  format: yaml
  label: ClassQuill Curriculum API
  slug: classquill-com-curriculum-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classquill-com/openapi/classquill-com-curriculum-api-openapi.yml
- filename: classquill-com-general-api-openapi.yml
  format: yaml
  label: ClassQuill General API
  slug: classquill-com-general-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classquill-com/openapi/classquill-com-general-api-openapi.yml
- filename: classquill-com-operations-api-openapi.yml
  format: yaml
  label: ClassQuill Operations API
  slug: classquill-com-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classquill-com/openapi/classquill-com-operations-api-openapi.yml
- filename: classquill-com-pricing-api-openapi.yml
  format: yaml
  label: ClassQuill Pricing API
  slug: classquill-com-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classquill-com/openapi/classquill-com-pricing-api-openapi.yml
- filename: classquill-com-reports-api-openapi.yml
  format: yaml
  label: ClassQuill Reports API
  slug: classquill-com-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classquill-com/openapi/classquill-com-reports-api-openapi.yml
- filename: classquill-com-sessions-api-openapi.yml
  format: yaml
  label: ClassQuill Sessions API
  slug: classquill-com-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classquill-com/openapi/classquill-com-sessions-api-openapi.yml
- filename: classquill-com-students-parents-api-openapi.yml
  format: yaml
  label: ClassQuill Students & Parents API
  slug: classquill-com-students-parents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classquill-com/openapi/classquill-com-students-parents-api-openapi.yml
- filename: classquill-com-tutors-api-openapi.yml
  format: yaml
  label: ClassQuill Tutors API
  slug: classquill-com-tutors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classquill-com/openapi/classquill-com-tutors-api-openapi.yml
auth_types: []
description: ClassQuill uses an API key authentication scheme.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ClassQuill Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClassQuill declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ClassQuill
provider_slug: classquill-com
scheme_count: 1
schemes:
- evidence: All API requests require an API key.
  header: Authorization
  how_to_obtain: Create a new key in Settings → Developers as an org owner or admin; the key is shown once and must be copied.
  location: header
  name: API Key
  scopes:
  - read
  - payments:write
  - tutors:write
  - payroll:write
  - coursework:write
  - sessions:write
  - accounts:write
  - write
  type: apiKey
slug: classquill-com-authentication
source_filename: classquill-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.classquill.com/authentication.md
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.classquill.com/authentication.md\nsources:\n- https://docs.classquill.com/authentication.md\n- https://docs.classquill.com/guides/org-setup.md\n- https://docs.classquill.com/quickstart.md\ndescription: ClassQuill uses an API key authentication scheme.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: All API requests require an API key.\n  location: header\n  header: Authorization\n  scopes:\n  - read\n  - payments:write\n  - tutors:write\n  - payroll:write\n  - coursework:write\n  - sessions:write\n  - accounts:write\n  - write\n  how_to_obtain: Create a new key in Settings → Developers as an org owner or admin; the key is shown once and must be copied.\ndocs: https://docs.classquill.com/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/classquill-com/authentication/classquill-com-authentication.yml
summary_line: 1 scheme
tags:
- Tutoring
- Scheduling
- Invoicing
- Payroll
- Learning Platform
- Education
---
