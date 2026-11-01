---
anonymous_access: false
api_key_in: []
auth_types: []
description: FastAPI Cloud uses Deploy Tokens for authentication when deploying applications via CLI or CI/CD.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fastapi Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: FastAPI Labs declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: FastAPI Labs
provider_slug: fastapi-labs
scheme_count: 2
schemes:
- evidence: Deploy tokens let you deploy your applications to FastAPI Cloud from CI/CD systems without using your personal account credentials.
  how_to_obtain: Create a Deploy Token in the FastAPI Cloud dashboard (Navigate to your app → Tokens → Create Token) and copy the displayed token value.
  location: environment
  name: FASTAPI_CLOUD_TOKEN
  type: apiKey
- evidence: 'Once you have a deploy token, set it along with your app ID as environment variables:'
  how_to_obtain: Copy the App ID (UUID) from the FastAPI Cloud dashboard header of your app.
  location: environment
  name: FASTAPI_CLOUD_APP_ID
  type: apiKey
slug: fastapi-labs-authentication
source_filename: fastapi-labs-authentication.yml
source_heading: Authentication Profile
source_url: https://fastapicloud.com/docs/advanced-features/deploy-tokens/
source_yaml: "generated: '2026-10-23'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://fastapicloud.com/docs/advanced-features/deploy-tokens/\nsources:\n- https://fastapicloud.com/docs/advanced-features/deploy-tokens/\n- https://fastapicloud.com/docs/getting-started/\n- https://fastapicloud.com/docs/getting-started/existing-project/\n- https://fastapicloud.com/docs/fastapi-cloud-cli/setup-ci/\ndescription: FastAPI Cloud uses Deploy Tokens for authentication when deploying applications via CLI or CI/CD.\nschemes:\n- type: apiKey\n  name: FASTAPI_CLOUD_TOKEN\n  evidence: Deploy tokens let you deploy your applications to FastAPI Cloud from CI/CD systems without using your personal account credentials.\n  location: environment\n  how_to_obtain: Create a Deploy Token in the FastAPI Cloud dashboard (Navigate to your app → Tokens → Create Token) and copy the displayed token\n    value.\n- type: apiKey\n  name: FASTAPI_CLOUD_APP_ID\n  evidence: 'Once you have a deploy\
  \ token, set it along with your app ID as environment variables:'\n  location: environment\n  how_to_obtain: Copy the App ID (UUID) from the FastAPI Cloud dashboard header of your app.\nnote: No OAuth2, HTTP bearer, or other authentication schemes are documented on the provided pages.\ndocs: https://fastapicloud.com/docs/advanced-features/deploy-tokens/\n"
source_yaml_url: https://artifacts.apis.io/fastapi-labs/authentication/fastapi-labs-authentication.yml
summary_line: 2 schemes
tags:
- Company
- API Platform
- Cloud
- Python
- Open Source
---
