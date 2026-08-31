---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Double Robotics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Double Robotics secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Double Robotics
provider_slug: double-robotics
scheme_count: 2
schemes:
- applies_to: Fleet REST API
  description: The Fleet REST API is authenticated with API keys issued through the Fleet Management account portal (drive.doublerobotics.com). Keys authorize access to fleet-management data — robots, users, call logs, and visitor passes.
  in: header
  name: FleetApiKey
  source: https://www.doublerobotics.com/developer.html
  type: apiKey
- applies_to: Double 3 SDK
  description: The Double 3 SDK is a LOCAL command/event API reached over a Unix domain socket on the robot itself; access is gated by putting the device into developer mode rather than by a network credential. No network token is exchanged for the on-device socket.
  name: LocalSocket
  source: https://github.com/doublerobotics/d3-sdk/blob/master/docs/Communication.md
  type: none
slug: double-robotics-authentication
source_filename: double-robotics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.doublerobotics.com/developer.html\ndocs: https://www.doublerobotics.com/developer.html\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  notes: >-\n    Double Robotics has no published OpenAPI, so this profile is derived from\n    the public developer documentation rather than a machine-readable spec.\nschemes:\n- name: FleetApiKey\n  type: apiKey\n  in: header\n  applies_to: Fleet REST API\n  description: >-\n    The Fleet REST API is authenticated with API keys issued through the Fleet\n    Management account portal (drive.doublerobotics.com). Keys authorize access\n    to fleet-management data — robots, users, call logs, and visitor passes.\n  source: https://www.doublerobotics.com/developer.html\n- name: LocalSocket\n  type: none\n  applies_to: Double 3 SDK\n  description: >-\n    The Double 3 SDK is a LOCAL command/event API reached over a Unix domain\n    socket on the robot itself; access is gated by\
  \ putting the device into\n    developer mode rather than by a network credential. No network token is\n    exchanged for the on-device socket.\n  source: https://github.com/doublerobotics/d3-sdk/blob/master/docs/Communication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/double-robotics/refs/heads/main/authentication/double-robotics-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Telepresence
- Robotics
- Videoconferencing
- Hybrid Work
- SDK
- Fleet Management
- Hardware
---
