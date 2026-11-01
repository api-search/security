---
anonymous_access: false
api_key_in: []
api_specs:
- filename: codecov-branches-api-openapi.yml
  format: yaml
  label: Codecov Branches API
  slug: codecov-branches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-branches-api-openapi.yml
- filename: codecov-commits-api-openapi.yml
  format: yaml
  label: Codecov Commits API
  slug: codecov-commits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-commits-api-openapi.yml
- filename: codecov-comparison-api-openapi.yml
  format: yaml
  label: Codecov Comparison API
  slug: codecov-comparison-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-comparison-api-openapi.yml
- filename: codecov-components-api-openapi.yml
  format: yaml
  label: Codecov Components API
  slug: codecov-components-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-components-api-openapi.yml
- filename: codecov-coverage-api-openapi.yml
  format: yaml
  label: Codecov Coverage API
  slug: codecov-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-coverage-api-openapi.yml
- filename: codecov-evaluations-api-openapi.yml
  format: yaml
  label: Codecov Evaluations API
  slug: codecov-evaluations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-evaluations-api-openapi.yml
- filename: codecov-flags-api-openapi.yml
  format: yaml
  label: Codecov Flags API
  slug: codecov-flags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-flags-api-openapi.yml
- filename: codecov-pulls-api-openapi.yml
  format: yaml
  label: Codecov Pulls API
  slug: codecov-pulls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-pulls-api-openapi.yml
- filename: codecov-repos-api-openapi.yml
  format: yaml
  label: Codecov Repos API
  slug: codecov-repos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-repos-api-openapi.yml
- filename: codecov-test-analytics-api-openapi.yml
  format: yaml
  label: Codecov Test Analytics API
  slug: codecov-test-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-test-analytics-api-openapi.yml
- filename: codecov-test-results-api-openapi.yml
  format: yaml
  label: Codecov Test Results API
  slug: codecov-test-results-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-test-results-api-openapi.yml
- filename: codecov-users-api-openapi.yml
  format: yaml
  label: Codecov Users API
  slug: codecov-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-users-api-openapi.yml
auth_types: []
description: Authentication schemes for Codecov self‑hosted OAuth login
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Codecov Authentication
name_suffix: Authentication
oauth_flows: []
overview: Codecov declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Codecov
provider_slug: codecov
scheme_count: 5
schemes:
- evidence: Store the **Client ID** and **Client Secret** for use in the configuration below
  how_to_obtain: Create a new GitHub App and copy the Client ID and Client Secret
  name: github
  type: oauth2
- evidence: Store the **Client ID** and **Client Secret** for use in the configuration below
  how_to_obtain: Create a new GitHub App on your Enterprise instance and copy the Client ID and Client Secret
  name: github_enterprise
  type: oauth2
- evidence: Copy the **Key** and **Secret** for your codecov.yml
  how_to_obtain: Add an OAuth consumer in Bitbucket.org and copy the Key and Secret
  name: bitbucket
  type: oauth2
- evidence: Append the information collected in step 1 in your self‑hosted `codecov.yml`.
  how_to_obtain: Create a new Application Link in Bitbucket Server and use the generated Consumer Key as client_id
  name: bitbucket_server
  type: oauth2
- evidence: Store the **Application Id** and **Secret** for use in the configuration below
  how_to_obtain: Create a new application in GitLab Enterprise and copy the Application Id and Secret
  name: gitlab_enterprise
  type: oauth2
slug: codecov-authentication
source_filename: codecov-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.codecov.com/docs/set-up-oauth-login.md
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.codecov.com/docs/set-up-oauth-login.md\nsources:\n- https://docs.codecov.com/docs/set-up-oauth-login.md\n- https://docs.codecov.com/docs/github-oauth-application-authorization\n- https://docs.codecov.com/docs/set-up-oauth-login\n- https://docs.codecov.com/docs/codecov-tokens.md\ndescription: Authentication schemes for Codecov self‑hosted OAuth login\nschemes:\n- type: oauth2\n  name: github\n  evidence: Store the **Client ID** and **Client Secret** for use in the configuration below\n  how_to_obtain: Create a new GitHub App and copy the Client ID and Client Secret\n- type: oauth2\n  name: github_enterprise\n  evidence: Store the **Client ID** and **Client Secret** for use in the configuration below\n  how_to_obtain: Create a new GitHub App on your Enterprise instance and copy the Client ID and Client Secret\n- type: oauth2\n  name: bitbucket\n  evidence: Copy the **Key**\
  \ and **Secret** for your codecov.yml\n  how_to_obtain: Add an OAuth consumer in Bitbucket.org and copy the Key and Secret\n- type: oauth2\n  name: bitbucket_server\n  evidence: Append the information collected in step 1 in your self‑hosted `codecov.yml`.\n  how_to_obtain: Create a new Application Link in Bitbucket Server and use the generated Consumer Key as client_id\n- type: oauth2\n  name: gitlab_enterprise\n  evidence: Store the **Application Id** and **Secret** for use in the configuration below\n  how_to_obtain: Create a new application in GitLab Enterprise and copy the Application Id and Secret\ndocs: https://docs.codecov.com/docs/set-up-oauth-login.md\n"
source_yaml_url: https://artifacts.apis.io/codecov/authentication/codecov-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Code Coverage
- CI/CD
- DevOps
- Testing
- Analytics
---
