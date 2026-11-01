---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication is performed by including two required headers in every request.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Getmeadow Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Meadow declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Meadow
provider_slug: getmeadow-com
scheme_count: 2
schemes:
- evidence: 'Every request must be authenticated by sending these two headers:'
  header: X-Consumer-Key
  how_to_obtain: A string that will be provided to you by a Meadow representative
  location: header
  name: X-Consumer-Key
  type: apiKey
- evidence: 'Every request must be authenticated by sending these two headers:'
  header: X-Client-Key
  how_to_obtain: A string that will be generated in the Meadow UI by a mutual client of Meadow and your company
  location: header
  name: X-Client-Key
  type: apiKey
slug: getmeadow-com-authentication
source_filename: getmeadow-com-authentication.yml
source_heading: Authentication Profile
source_url: https://api-docs.getmeadow.com/authentication.md
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api-docs.getmeadow.com/authentication.md\nsources:\n- https://api-docs.getmeadow.com/authentication.md\ndescription: Authentication is performed by including two required headers in every request.\nschemes:\n- type: apiKey\n  name: X-Consumer-Key\n  evidence: 'Every request must be authenticated by sending these two headers:'\n  location: header\n  header: X-Consumer-Key\n  how_to_obtain: A string that will be provided to you by a Meadow representative\n- type: apiKey\n  name: X-Client-Key\n  evidence: 'Every request must be authenticated by sending these two headers:'\n  location: header\n  header: X-Client-Key\n  how_to_obtain: A string that will be generated in the Meadow UI by a mutual client of Meadow and your company\ndocs: https://api-docs.getmeadow.com/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/getmeadow-com/authentication/getmeadow-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Cannabis
- POS
- E-commerce
- SaaS
---
