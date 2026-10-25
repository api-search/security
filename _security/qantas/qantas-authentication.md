---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: none
name: Qantas Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qantas declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Qantas
provider_slug: qantas
scheme_count: 0
schemes: []
slug: qantas-authentication
source_filename: qantas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: none\nsource: conventions/qantas-conventions.yml (authentication block, from Qantas Agency Connect docs read 2026-07-28)\ndocs: https://agencyconnect.qantas.com/en-au/ndc/distribution-platform-portal/knowledge-centre/access-credentials-and-password-management\nschemes: []\nnote: |\n  Checked: Qantas publishes no authentication scheme for the Qantas Distribution Platform NDC XML API --\n  no OpenAPI securityScheme, no OAuth/API-key documentation, no token endpoint. Credentials are\n  bilateral, issued after a signed Qantas Distribution Platform Access Agreement. The only documented\n  credentials are for the QDP portal (a web UI powered by Accelya NDC SPRK), which issues per-consultant\n  access credentials with two-factor authentication; that is a human login, not an API scheme.\n  No OAuth is documented, so no scopes/ artifact is written.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qantas/refs/heads/main/authentication/qantas-authentication.yml
summary_line: 0 schemes
tags:
- Travel
- Australia
- Aviation
- Airlines
- Distribution
- NDC
- Booking
- Corporate Travel
- Loyalty
---
