---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Approvecom Authentication
name_suffix: Authentication
oauth_flows: []
overview: Approve.com secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Approve.com
provider_slug: approvecom
scheme_count: 1
schemes:
- description: Every Approve.com / Tipalti Procurement REST API request must include the API token in the x-api-key header. Tokens are issued per environment (sandbox and production) and are obtained from your Tipalti Implementation Manager rather than a self-serve dashboard.
  environments:
  - base_url: https://triggers.approve.com
    name: production
  - base_url: https://triggers.sandbox.approve.com
    name: sandbox
  in: header
  name: ApiKeyAuth
  parameter_name: x-api-key
  type: apiKey
slug: approvecom-authentication
source_filename: approvecom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://help.tipalti.com/hc/en-us/articles/30718248220823-Procurement-REST-API-documentation\ndocs: https://help.tipalti.com/hc/en-us/articles/30718248220823-Procurement-REST-API-documentation\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  description: >-\n    Every Approve.com / Tipalti Procurement REST API request must include the API token in\n    the x-api-key header. Tokens are issued per environment (sandbox and production) and are\n    obtained from your Tipalti Implementation Manager rather than a self-serve dashboard.\n  environments:\n  - name: production\n    base_url: https://triggers.approve.com\n  - name: sandbox\n    base_url: https://triggers.sandbox.approve.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/approvecom/refs/heads/main/authentication/approvecom-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Procurement
- Purchase Orders
- Spend Management
- Accounts Payable
- Vendor Management
- Finance
- Approvals
- B2B
---
