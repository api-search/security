---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pdfbroker-io-pdf-api-openapi.yml
  format: yaml
  label: pdfbroker-io PDF API
  slug: pdfbroker-io-pdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pdfbroker-io/openapi/pdfbroker-io-pdf-api-openapi.yml
auth_types: []
description: Authentication schemes for PdfBroker.io API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Pdfbroker Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: pdfbroker-io declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: pdfbroker-io
provider_slug: pdfbroker-io
scheme_count: 1
schemes:
- evidence: The PdfBroker.io API uses OAuth 2.0 with the client credentials grant type.
  flows:
  - client_credentials
  how_to_obtain: client_id and client_secret are found in Members > API
  name: OAuth 2.0
  scopes:
  - pdfbroker
  token_url: https://login.pdfbroker.io/connect/token
  type: oauth2
slug: pdfbroker-io-authentication
source_filename: pdfbroker-io-authentication.yml
source_heading: Authentication Profile
source_url: https://www.pdfbroker.io/docs/authentication
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.pdfbroker.io/docs/authentication\nsources:\n- https://www.pdfbroker.io/docs/authentication\n- https://www.pdfbroker.io/docs/getting-started\ndescription: Authentication schemes for PdfBroker.io API\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: The PdfBroker.io API uses OAuth 2.0 with the client credentials grant type.\n  flows:\n  - client_credentials\n  token_url: https://login.pdfbroker.io/connect/token\n  scopes:\n  - pdfbroker\n  how_to_obtain: client_id and client_secret are found in Members > API\ndocs: https://www.pdfbroker.io/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/pdfbroker-io/authentication/pdfbroker-io-authentication.yml
summary_line: 1 scheme
tags:
- PDF Generation
- REST API
- HTML to PDF
- PDF/A
- PDF/UA
- PDF Utilities
- XSL-FO
---
