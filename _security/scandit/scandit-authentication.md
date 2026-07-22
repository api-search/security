---
api_key_in:
- sdk-configuration
auth_types:
- licenseKey
description: ''
kind: authentication
layout: security
method: searched
name: Scandit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scandit secures its APIs with licenseKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Scandit
provider_slug: scandit
scheme_count: 2
schemes:
- gates:
  - barcode
  - matrixscan
  - id
  - smart-label
  - parser
  - text
  location: sdk-initialization
  name: licenseKey
  provisioning: https://ssl.scandit.com/dashboard/
  scope: application (bundle id / package name / web origin)
  type: license-key
- name: idBoltClientKey
  note: ID Bolt sessions are configured with a Scandit license key passed to IdBoltSession.
  product: ID Bolt (hosted)
  type: license-key
slug: scandit-authentication
source_filename: scandit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.scandit.com/ (SDK licensing / getting-started)\ndocs: https://docs.scandit.com/\nsummary:\n  types: [licenseKey]\n  api_key_in: [sdk-configuration]\n  oauth2_flows: []\nnote: >-\n  Scandit does not expose a REST API secured by OAuth or API keys. Authentication\n  is a per-application LICENSE KEY provisioned from the Scandit dashboard and\n  supplied to the Data Capture SDK at initialization (e.g. DataCaptureContext /\n  ScanditLicense). Keys are scoped to an app bundle id / package name / web origin\n  and gate which products (Barcode, MatrixScan, ID, Smart Label, Parser) are\n  enabled. There are no OAuth scopes.\nschemes:\n  - name: licenseKey\n    type: license-key\n    location: sdk-initialization\n    provisioning: https://ssl.scandit.com/dashboard/\n    scope: application (bundle id / package name / web origin)\n    gates: [barcode, matrixscan, id, smart-label, parser, text]\n  - name: idBoltClientKey\n \
  \   type: license-key\n    product: ID Bolt (hosted)\n    note: ID Bolt sessions are configured with a Scandit license key passed to IdBoltSession.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scandit/refs/heads/main/authentication/scandit-authentication.yml
summary_line: licenseKey · 2 schemes
tags:
- Company
- Frontier Tech
- Data Capture
- Barcode Scanning
- Computer Vision
- SDK
- ID Verification
- Retail
- Logistics
- Mobile
---
