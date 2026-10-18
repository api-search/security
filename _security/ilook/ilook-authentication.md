---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for iLook AI Face Analysis
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ilook Authentication
name_suffix: Authentication
oauth_flows: []
overview: iLook AI Face Analysis (Wallic Technologies) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: iLook AI Face Analysis (Wallic Technologies)
provider_slug: ilook
scheme_count: 1
schemes:
- evidence: 'Send the issued key in the HTTP header:

    `Authorization: Bearer <api-key>`'
  header: Authorization
  how_to_obtain: Beta API keys are issued out of band by the ilook operator.
  location: header
  name: Bearer
  type: http-bearer
slug: ilook-authentication
source_filename: ilook-authentication.yml
source_heading: Authentication Profile
source_url: https://www.ilook.fit/auth.md
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.ilook.fit/auth.md\nsources:\n- https://www.ilook.fit/auth.md\ndescription: Authentication schemes for iLook AI Face Analysis\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send the issued key in the HTTP header:\n\n    `Authorization: Bearer <api-key>`'\n  location: header\n  header: Authorization\n  how_to_obtain: Beta API keys are issued out of band by the ilook operator.\ndocs: https://www.ilook.fit/auth.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ilook/refs/heads/main/authentication/ilook-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- FaceAnalysis
- ImageProcessing
- Biometrics
---
