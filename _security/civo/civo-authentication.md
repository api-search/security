---
anonymous_access: false
api_key_in: []
api_specs:
- filename: civo-openapi-generated.yml
  format: yaml
  label: Civo API
  slug: civo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/civo/openapi/_ae-authored/civo-openapi-generated.yml
auth_types: []
description: Civo provides API key authentication for its main API and CLI, and S3-style credentials for object store access.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Civo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Civo declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Civo
provider_slug: civo
scheme_count: 2
schemes:
- evidence: To authenticate the account for the API or tools that use it such as the Civo command-line interface, you will need to provide an API key that is unique to your account.
  header: Authorization
  how_to_obtain: In order to acquire the API key for an account, navigate to the Profile/Security section of your Civo account.
  location: header
  name: API Key
  type: apiKey
- evidence: To access object store contents through the S3 API, you will need to create a credential that can be associated with the store.
  how_to_obtain: 'On the credentials management page, you can drop down on the credential of your choosing to list its details: This detail page shows two pieces of information for the credential: The Access Key ID, The hidden secret key'
  name: S3 Credentials
  type: other
slug: civo-authentication
source_filename: civo-authentication.yml
source_heading: Authentication Profile
source_url: https://www.civo.com/docs/account/api-keys
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (deepseek)\nsource: https://www.civo.com/docs/account/api-keys\nsources:\n- https://www.civo.com/docs/account/api-keys\n- https://www.civo.com/docs/account/signing-up\n- https://www.civo.com/docs/object-stores/object-store-credentials\n- https://www.civo.com/docs/database/getting-started\ndescription: Civo provides API key authentication for its main API and CLI, and S3-style credentials for object store access.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: To authenticate the account for the API or tools that use it such as the Civo command-line interface, you will need to provide an\n    API key that is unique to your account.\n  header: Authorization\n  location: header\n  how_to_obtain: In order to acquire the API key for an account, navigate to the Profile/Security section of your Civo account.\n- type: other\n  name: S3 Credentials\n  evidence: To access object store contents through\
  \ the S3 API, you will need to create a credential that can be associated with the store.\n  how_to_obtain: 'On the credentials management page, you can drop down on the credential of your choosing to list its details: This detail page\n    shows two pieces of information for the credential: The Access Key ID, The hidden secret key'\ndocs: https://www.civo.com/docs/account/api-keys, https://www.civo.com/docs/object-stores/object-store-credentials\nnote: The API key documentation doesn't explicitly state the header name or location, but based on common API patterns and the evidence stating\n  it's used to \"authenticate you for tools that interact with the Civo API\", it's reasonable to infer it goes in the Authorization header. The\n  S3 credentials are for accessing object stores via S3 API.\n"
source_yaml_url: https://artifacts.apis.io/civo/authentication/civo-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Cloud
- Kubernetes
- Cloud Computing
- Infrastructure
- Artificial Intelligence
- GPU
- Sovereign Cloud
---
