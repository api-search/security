---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Hailo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hailo declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Hailo
provider_slug: hailo
scheme_count: 0
schemes: []
slug: hailo-authentication
source_filename: hailo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: derived\nsource: grpc/hailo-media-library-service.proto, grpc/hailo-hailort-hrpc.proto, skills/hailo-connect.md\nnote: >-\n  derive-authentication.py was not run because it reads OpenAPI securitySchemes and Hailo publishes no\n  OpenAPI. This profile is derived from the saved Protocol Buffers contracts and from Hailo's own\n  published skill documentation. Hailo has NO network API and therefore no API keys, OAuth flows, JWTs\n  or token endpoints of any kind — the surfaces below are locally authenticated by the operating system.\n  Nothing here is a vulnerability report; every value is published by Hailo in its own public repository.\nschemes: []\nscheme_count: 0\nnetwork_authentication: none\nlocal_access_model:\n- surface: HailoRT library / hailortcli\n  transport: PCIe (kernel driver) or USB\n  authentication: OS file permissions on the /dev/hailo* device nodes; no application-level credential.\n  evidence: https://github.com/hailo-ai/hailort-drivers\n\
  - surface: MediaLibraryService gRPC\n  transport: local gRPC socket on the Hailo-15 board\n  authentication: >-\n    None declared in the contract. grpc/hailo-media-library-service.proto defines no credential, token\n    or metadata field on any of its 33 RPCs; the service is reachable only from the board.\n  evidence: grpc/hailo-media-library-service.proto\n- surface: Hailo-15 SBC shell\n  transport: SSH over ethernet\n  authentication: >-\n    Password. Hailo's own published skill states the board's factory default is root / root at\n    10.0.0.1 — a documented development default, quoted here from the provider's public repository.\n  evidence: https://github.com/hailo-ai/hailo15-agentic-coding/blob/main/.claude/skills/connect/SKILL.md\n- surface: Hailo Developer Zone downloads\n  transport: HTTPS\n  authentication: Account registration (form-gated), required to download the Dataflow Compiler, HailoRT wheels and .deb packages.\n  evidence: https://hailo.ai/developer-zone/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hailo/refs/heads/main/authentication/hailo-authentication.yml
summary_line: 0 schemes
tags:
- Artificial Intelligence
- Machine Learning
- Semiconductors
- Edge Computing
- Computer Vision
- Inference
- Embedded Systems
- Video Analytics
- Hardware
- Generative AI
- Protocol Buffers
- gRPC
---
