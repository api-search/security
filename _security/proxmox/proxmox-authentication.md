---
api_key_in:
- cookie
- header
api_specs:
- filename: proxmox-openapi.yml
  format: yaml
  label: Proxmox VE API
  slug: ve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/proxmox/refs/heads/main/openapi/proxmox-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Proxmox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Proxmox VE secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Proxmox VE
provider_slug: proxmox
scheme_count: 2
schemes:
- description: 'Stateless API token. Send header

    `Authorization: PVEAPIToken=USER@REALM!TOKENID=UUID`.

    No CSRFPreventionToken required.'
  in: header
  name: apiTokenAuth
  parameter: Authorization
  sources:
  - openapi/proxmox-openapi.yml
  type: apiKey
- description: 'Ticket issued by POST /access/ticket. Carried as a cookie. Write

    operations also require the `CSRFPreventionToken` header returned with

    the ticket. Tickets expire after 2 hours.'
  in: cookie
  name: ticketAuth
  parameter: PVEAuthCookie
  sources:
  - openapi/proxmox-openapi.yml
  type: apiKey
slug: proxmox-authentication
source_filename: proxmox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/proxmox-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: apiTokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Stateless API token. Send header\n    `Authorization: PVEAPIToken=USER@REALM!TOKENID=UUID`.\n    No CSRFPreventionToken required.\n  sources:\n  - openapi/proxmox-openapi.yml\n- name: ticketAuth\n  type: apiKey\n  in: cookie\n  parameter: PVEAuthCookie\n  description: |-\n    Ticket issued by POST /access/ticket. Carried as a cookie. Write\n    operations also require the `CSRFPreventionToken` header returned with\n    the ticket. Tickets expire after 2 hours.\n  sources:\n  - openapi/proxmox-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proxmox/refs/heads/main/authentication/proxmox-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Virtualization
- KVM
- Containers
- LXC
- Clustering
- Open Source
---
