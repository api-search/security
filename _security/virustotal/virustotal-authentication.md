---
api_key_in:
- header
api_specs:
- filename: virustotal-access-control-openapi.yml
  format: yaml
  label: VirusTotal API v3 - Access Control
  slug: virustotal-api-v3-access-control
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/openapi/virustotal-access-control-openapi.yml
- filename: virustotal-ioc-feeds-openapi.yml
  format: yaml
  label: VirusTotal API v3 - IoC Feeds
  slug: virustotal-api-v3-ioc-feeds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/openapi/virustotal-ioc-feeds-openapi.yml
- filename: virustotal-ioc-investigation-openapi.yml
  format: yaml
  label: VirusTotal API v3 - IoC Investigation
  slug: virustotal-api-v3-ioc-investigation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/openapi/virustotal-ioc-investigation-openapi.yml
- filename: virustotal-private-scanning-openapi.yml
  format: yaml
  label: VirusTotal API v3 - Private Scanning
  slug: virustotal-api-v3-private-scanning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/openapi/virustotal-private-scanning-openapi.yml
- filename: virustotal-threat-graphs-openapi.yml
  format: yaml
  label: VirusTotal API v3 - Threat Graphs
  slug: virustotal-api-v3-threat-graphs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/openapi/virustotal-threat-graphs-openapi.yml
- filename: virustotal-threat-landscape-openapi.yml
  format: yaml
  label: VirusTotal API v3 - Threat Landscape & Vulnerability Intelligence
  slug: virustotal-api-v3-threat-landscape-vulnerability-intelligence
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/openapi/virustotal-threat-landscape-openapi.yml
- filename: virustotal-yara-hunting-openapi.yml
  format: yaml
  label: VirusTotal API v3 - YARA Hunting (Livehunt, Retrohunt, IoC Stream)
  slug: virustotal-api-v3-yara-hunting-livehunt-retrohunt-ioc-stream
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/openapi/virustotal-yara-hunting-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Virustotal Authentication
name_suffix: Authentication
oauth_flows: []
overview: VirusTotal secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: VirusTotal
provider_slug: virustotal
scheme_count: 1
schemes:
- description: Personal VirusTotal / GTI API key. Found in the user menu of your VirusTotal account.
  in: header
  name: VTApiKey
  parameter: x-apikey
  sources:
  - openapi/virustotal-access-control-openapi.yml
  - openapi/virustotal-ioc-feeds-openapi.yml
  - openapi/virustotal-ioc-investigation-openapi.yml
  - openapi/virustotal-private-scanning-openapi.yml
  - openapi/virustotal-threat-graphs-openapi.yml
  - openapi/virustotal-threat-landscape-openapi.yml
  - openapi/virustotal-yara-hunting-openapi.yml
  type: apiKey
slug: virustotal-authentication
source_filename: virustotal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/virustotal-access-control-openapi.yml, openapi/virustotal-ioc-feeds-openapi.yml,\n  openapi/virustotal-ioc-investigation-openapi.yml, openapi/virustotal-private-scanning-openapi.yml,\n  openapi/virustotal-threat-graphs-openapi.yml, openapi/virustotal-threat-landscape-openapi.yml,\n  openapi/virustotal-yara-hunting-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: VTApiKey\n  type: apiKey\n  in: header\n  parameter: x-apikey\n  description: Personal VirusTotal / GTI API key. Found in the user menu of your VirusTotal\n    account.\n  sources:\n  - openapi/virustotal-access-control-openapi.yml\n  - openapi/virustotal-ioc-feeds-openapi.yml\n  - openapi/virustotal-ioc-investigation-openapi.yml\n  - openapi/virustotal-private-scanning-openapi.yml\n  - openapi/virustotal-threat-graphs-openapi.yml\n  - openapi/virustotal-threat-landscape-openapi.yml\n  - openapi/virustotal-yara-hunting-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/authentication/virustotal-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Anti-Malware
- Threat Intelligence
- Security
- File Analysis
- URL Analysis
- YARA
- IoC
- Sandbox
- MITRE ATT&CK
- Google Cloud
---
