---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Cloud HPC Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloud HPC declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Cloud HPC
provider_slug: cloudhpc-cloud
scheme_count: 3
schemes:
- applies_to: API v2 (https://cloud.cfdfeaservice.it/api/v2)
  evidence: 'Your APIKEY is on your profile page . It must be passed to EVERY API call as a header. The correct way to do this is: -H ''X-API-key: $apikey'''
  header: X-API-key
  in: header
  name: X-API-key
  type: apiKey
- applies_to: API v1 (legacy)
  evidence: Every API accepts the API_KEY either in the URL or in the HEADER of the call ... We recommend passing the API_KEY in the HEADER.
  header: api-key
  in: header
  name: api-key
  type: apiKey
- applies_to: API v1 (legacy)
  evidence: '''https://cloud.cfdfeaservice.it/api/v{version}/simulation?api_key={api_key}'
  in: query
  name: api_key (query)
  parameter: api_key
  type: apiKey
slug: cloudhpc-cloud-authentication
source_filename: cloudhpc-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://docs.cloudhpc.cloud/API-v2/\ndocs: https://docs.cloudhpc.cloud/APIKEY/\ndocs_related:\n- https://docs.cloudhpc.cloud/API-v2/\n- https://docs.cloudhpc.cloud/API-v1/\nschemes:\n- name: X-API-key\n  type: apiKey\n  in: header\n  header: X-API-key\n  applies_to: API v2 (https://cloud.cfdfeaservice.it/api/v2)\n  evidence: \"Your APIKEY is on your profile page . It must be passed to EVERY API call as a header. The correct way to do this is: -H 'X-API-key: $apikey'\"\n- name: api-key\n  type: apiKey\n  in: header\n  header: api-key\n  applies_to: API v1 (legacy)\n  evidence: \"Every API accepts the API_KEY either in the URL or in the HEADER of the call ... We recommend passing the API_KEY in the HEADER.\"\n- name: api_key (query)\n  type: apiKey\n  in: query\n  parameter: api_key\n  applies_to: API v1 (legacy)\n  evidence: \"'https://cloud.cfdfeaservice.it/api/v{version}/simulation?api_key={api_key}\"\nkey_management:\n  issuance:\
  \ 'Every account is assigned its own APIKEY when it is created. Shown on the account profile page; a JSON license file with username and apikey is also provided.'\n  scope: 'Sharing your APIKEY with someone gives them full access to your account (no scoped keys documented).'\n  rotation: The MCP server README says regenerating the API key in the cloudHPC profile revokes access for connected assistants.\n  availability: 'The API may not be available on the FREE plan (i.e. while using the initial 300 vCPU Hours).; v2 access must be requested from support.'\nmcp_oauth:\n  note: The hosted MCP endpoint https://mcp.cloudhpc.cloud/mcp documents an OAuth sign-in (paste API key, optional read-only access, tokens expiring after one hour, renewed for 30 days) or an X-API-Key / Authorization Bearer header. This is the MCP connector, not the REST API.\n  source: https://github.com/CFD-FEA-SERVICE/cloudhpc-mcp\n"
source_yaml_url: https://artifacts.apis.io/cloudhpc-cloud/authentication/cloudhpc-cloud-authentication.yml
summary_line: 3 schemes
tags:
- Company
- High Performance Computing
- Cloud Computing
- Engineering Simulation
- CFD
- FEA
- CAE
- MCP
---
