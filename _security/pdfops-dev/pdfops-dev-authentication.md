---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Pdfops Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: pdfops-dev declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: pdfops-dev
provider_slug: pdfops-dev
scheme_count: 1
schemes:
- evidence: Every PDFops operation now sends the key as X-API-Key.
  header: X-API-Key
  how_to_obtain: Request a free API key via POST /api/signup; the key is emailed to the address you submit.
  location: header
  name: API Key
  type: apiKey
slug: pdfops-dev-authentication
source_filename: pdfops-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://pdfops.dev/docs/signup
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://pdfops.dev/docs/signup\nsources:\n- https://pdfops.dev/docs/signup\n- https://pdfops.dev/blog/fill-w9-from-webhook\n- https://pdfops.dev/blog/getting-started\n- https://pdfops.dev/use-cases/contracts\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Every PDFops operation now sends the key as X-API-Key.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Request a free API key via POST /api/signup; the key is emailed to the address you submit.\ndocs: https://pdfops.dev/docs/signup\n"
source_yaml_url: https://artifacts.apis.io/pdfops-dev/authentication/pdfops-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- API
- PDF
- AI
- No-code
- Python
---
