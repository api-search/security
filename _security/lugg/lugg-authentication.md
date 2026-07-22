---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Lugg Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lugg secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lugg
provider_slug: lugg
scheme_count: 1
schemes:
- evidence: Reference navigation exposes tag-group "authentication" and tag "oauth" (token issuance/management endpoints).
  name: OAuth
  source: https://docs.lugg.com
  type: oauth2
slug: lugg-authentication
source_filename: lugg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.lugg.com\ndocs: https://docs.lugg.com\nsummary:\n  types:\n  - oauth2\n  notes: >-\n    The Lugg API documents an OAuth-based authentication model. The reference\n    (docs.lugg.com) groups authentication under an \"Authentication\" tag group\n    with a dedicated \"OAuth\" resource for obtaining and managing access tokens.\n    The live API host is https://api.lugg.com (Render-backed; returns an\n    x-request-id on every response). Exact authorization/token URLs and scope\n    names are rendered client-side in the Scalar reference and were not\n    machine-extractable in this pass; capture them verbatim on the next run that\n    can read the underlying OpenAPI document.\nschemes:\n- name: OAuth\n  type: oauth2\n  source: https://docs.lugg.com\n  evidence: >-\n    Reference navigation exposes tag-group \"authentication\" and tag \"oauth\"\n    (token issuance/management endpoints).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lugg/refs/heads/main/authentication/lugg-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Logistics
- Delivery
- Moving
- Last Mile
- Transportation
- On-Demand
- Webhooks
---
