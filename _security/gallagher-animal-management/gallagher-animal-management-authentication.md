---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gallagher-animal-management-openapi-generated.yml
  format: yaml
  label: Gallagher API
  slug: gallagher-animal-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gallagher-animal-management/openapi/_ae-authored/gallagher-animal-management-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Gallagher Animal Management Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gallagher declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Gallagher
provider_slug: gallagher-animal-management
scheme_count: 2
schemes:
- description: Use a client certificate to authenticate REST API calls. The certificate thumbprint is entered in the REST client configuration.
  evidence: Create and assign a client certificate for REST API authentication.
  type: mutualTLS
- description: Thumbprint of the client certificate used for authentication.
  evidence: Copy the Thumbprint ... paste it into the Client Certificate Thumbprint field of the REST Client (API Key tab).
  in: header
  name: X-Client-Certificate-Thumbprint
  type: apiKey
slug: gallagher-animal-management-authentication
source_filename: gallagher-animal-management-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://help.security.gallagher.com/knowledge-hub/products/cc-software/configure/interface-options/api/representational-state-transfer-rest-api/rest-api-creating-the-client-certificate.md\nschemes:\n  - type: mutualTLS\n    description: Use a client certificate to authenticate REST API calls. The certificate thumbprint is entered in the REST client configuration.\n    evidence: \"Create and assign a client certificate for REST API authentication.\"\n  - type: apiKey\n    in: header\n    name: X-Client-Certificate-Thumbprint\n    description: Thumbprint of the client certificate used for authentication.\n    evidence: \"Copy the Thumbprint ... paste it into the Client Certificate Thumbprint field of the REST Client (API Key tab).\"\n"
source_yaml_url: https://artifacts.apis.io/gallagher-animal-management/authentication/gallagher-animal-management-authentication.yml
summary_line: 2 schemes
tags:
- Animal Management
- Electric Fencing
- Weighing
- EID
- Watering
- Security
---
