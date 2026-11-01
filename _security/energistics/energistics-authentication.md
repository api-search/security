---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods published by Energistics for ETP v1.1
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Energistics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Energistics declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Energistics
provider_slug: energistics
scheme_count: 3
schemes:
- evidence: 'The token MUST be presented using the Bearer schema. The content of the header should look something like this: Authorization: Bearer <token>'
  header: Authorization
  how_to_obtain: Implementation‑dependent; not specified on the page.
  location: header
  name: Bearer
  type: http-bearer
- evidence: The token is presented during the WebSocket upgrade request, using either the Authorization header or on the query string as described above.
  how_to_obtain: Implementation‑dependent; not specified on the page.
  location: query
  name: Bearer
  type: http-bearer
- evidence: Basic authentication is as described in RFC-2617 (https://www.ietf.org/rfc/rfc2617.txt) for HTTP connections.
  header: Authorization
  how_to_obtain: Standard HTTP Basic credentials (username and password) as defined in RFC‑2617.
  location: header
  name: Basic
  type: http-basic
slug: energistics-authentication
source_filename: energistics-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.energistics.org/ETP/ETP_TOPICS/ETP-000-171-0-C-sv1100.html
source_yaml: "generated: '2026-10-23'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.energistics.org/ETP/ETP_TOPICS/ETP-000-171-0-C-sv1100.html\nsources:\n- https://docs.energistics.org/ETP/ETP_TOPICS/ETP-000-171-0-C-sv1100.html\n- https://docs.energistics.org/ETP/ETP_TOPICS/ETP-000-172-0-C-sv1100.html\n- https://docs.energistics.org/ETP/ETP_TOPICS/ETP-000-177-0-C-sv1100.html\n- https://docs.energistics.org/ETP/ETP_TOPICS/ETP-000-173-0-C-sv1100.html\ndescription: Authentication methods published by Energistics for ETP v1.1\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'The token MUST be presented using the Bearer schema. The content of the header should look something like this: Authorization: Bearer\n    <token>'\n  location: header\n  header: Authorization\n  how_to_obtain: Implementation‑dependent; not specified on the page.\n- type: http-bearer\n  name: Bearer\n  evidence: The token is presented during the WebSocket upgrade request,\
  \ using either the Authorization header or on the query string as described\n    above.\n  location: query\n  how_to_obtain: Implementation‑dependent; not specified on the page.\n- type: http-basic\n  name: Basic\n  evidence: Basic authentication is as described in RFC-2617 (https://www.ietf.org/rfc/rfc2617.txt) for HTTP connections.\n  location: header\n  header: Authorization\n  how_to_obtain: Standard HTTP Basic credentials (username and password) as defined in RFC‑2617.\ndocs: https://docs.energistics.org/ETP/ETP_TOPICS/ETP-000-171-0-C-sv1100.html\n"
source_yaml_url: https://artifacts.apis.io/energistics/authentication/energistics-authentication.yml
summary_line: 3 schemes
tags:
- Data Standards
- Energy Industry
- Oil & Gas
- Non‑profit Consortium
- Data Interoperability
- Technical Standards
---
