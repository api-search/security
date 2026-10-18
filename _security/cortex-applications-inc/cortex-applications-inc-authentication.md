---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cortex-applications-inc-app-api-openapi.yml
  format: yaml
  label: Cortex Applications, Inc. App API
  slug: cortex-applications-inc-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cortex-applications-inc/refs/heads/main/openapi/cortex-applications-inc-app-api-openapi.yml
- filename: cortex-applications-inc-cities-api-openapi.yml
  format: yaml
  label: Cortex Applications, Inc. Cities API
  slug: cortex-applications-inc-cities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cortex-applications-inc/refs/heads/main/openapi/cortex-applications-inc-cities-api-openapi.yml
- filename: cortex-applications-inc-meta-api-openapi.yml
  format: yaml
  label: Cortex Applications, Inc. Meta API
  slug: cortex-applications-inc-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cortex-applications-inc/refs/heads/main/openapi/cortex-applications-inc-meta-api-openapi.yml
- filename: cortex-applications-inc-orgs-api-openapi.yml
  format: yaml
  label: Cortex Applications, Inc. Orgs API
  slug: cortex-applications-inc-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cortex-applications-inc/refs/heads/main/openapi/cortex-applications-inc-orgs-api-openapi.yml
- filename: cortex-applications-inc-repos-api-openapi.yml
  format: yaml
  label: Cortex Applications, Inc. Repos API
  slug: cortex-applications-inc-repos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cortex-applications-inc/refs/heads/main/openapi/cortex-applications-inc-repos-api-openapi.yml
auth_types: []
description: Authentication schemes used in the documented Cortex workflows
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cortex Applications Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cortex Applications, Inc. declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Cortex Applications, Inc.
provider_slug: cortex-applications-inc
scheme_count: 2
schemes:
- evidence: 'Authorization: "Bearer {{ context.secrets.pd_token }}"'
  header: Authorization
  how_to_obtain: Stored as a secret named `pd_token` in Cortex
  location: header
  name: PagerDuty token
  type: http-bearer
- evidence: 'Authorization: "Bearer {{ context.secrets.GITHUB_COPILOT_TOKEN }}"'
  header: Authorization
  how_to_obtain: Stored as a secret named `GITHUB_COPILOT_TOKEN` in Cortex
  location: header
  name: GitHub Copilot token
  type: http-bearer
slug: cortex-applications-inc-authentication
source_filename: cortex-applications-inc-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.cortex.io/guides/dev-onboarding/env-setup-workflow.md
source_yaml: "generated: '2026-10-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.cortex.io/guides/dev-onboarding/env-setup-workflow.md\nsources:\n- https://docs.cortex.io/guides/dev-onboarding/env-setup-workflow.md\n- https://docs.cortex.io/guides/dev-onboarding/automate-user-access-to-github-pagerduty-and-jira.md\n- https://docs.cortex.io/guides/dev-onboarding/automate-user-access-to-copilot.md\ndescription: Authentication schemes used in the documented Cortex workflows\nschemes:\n- type: http-bearer\n  name: PagerDuty token\n  evidence: 'Authorization: \"Bearer {{ context.secrets.pd_token }}\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Stored as a secret named `pd_token` in Cortex\n- type: http-bearer\n  name: GitHub Copilot token\n  evidence: 'Authorization: \"Bearer {{ context.secrets.GITHUB_COPILOT_TOKEN }}\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Stored as a secret named `GITHUB_COPILOT_TOKEN`\
  \ in Cortex\ndocs: https://docs.cortex.io/guides/dev-onboarding/env-setup-workflow.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cortex-applications-inc/refs/heads/main/authentication/cortex-applications-inc-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Engineering
- Platform
- Artificial Intelligence
- Developer Productivity
---
