---
api_specs:
- filename: kurrent-kurrentdb-http-api-openapi.yml
  format: yaml
  label: KurrentDB HTTP API
  slug: kurrentdb-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kurrent/refs/heads/main/openapi/kurrent-kurrentdb-http-api-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Kurrent Trust Center
name_suffix: Trust Center
overview: Kurrent maintains a public trust center covering its security and compliance posture.
provider_name: Kurrent
provider_slug: kurrent
slug: kurrent-trust-center
source_filename: kurrent-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nurl: https://trust.kurrent.io/\nnotes: >-\n  Kurrent operates a Trust Center at trust.kurrent.io, hosted on Vanta, and https://www.kurrent.io/security\n  redirects to it. The page renders its contents client-side, so the certification list could not\n  be extracted programmatically and NO named certification is asserted here. The automated probe\n  (0-working/probe-security-programs.py) therefore returned no keyword hit. This record captures\n  the verified existence and location of the trust surface only; a future pass with a rendering\n  fetch should fill certifications[].\ncertifications: []\nevidence:\n- source: https://trust.kurrent.io/\n  status: 200\n  kind: trust-center\n  detail: 'Page title: Kurrent Trust Center. Vanta-hosted, JavaScript-rendered.'\n- source: https://www.kurrent.io/security\n  status: 200\n  kind: redirect-to-trust-center\nsecurity_program:\n  fips_140:\n    claimed: true\n    evidence: >-\n\
  \      \"FIPS Compliance\" is listed among the features of the EventStoreDB 23.10 LTS release at\n      https://www.kurrent.io/releases\n  encryption_at_rest:\n    claimed: true\n    evidence: >-\n      Encryption at rest shipped in EventStoreDB 24.10, per https://www.kurrent.io/releases\n  cve_disclosure:\n    claimed: true\n    evidence: >-\n      Kurrent publishes security releases with CVE identifiers — the February 2024 release names\n      CVE-2024-26133 — through https://www.kurrent.io/releases\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kurrent/refs/heads/main/security/kurrent-trust-center.yml
summary_line: trust center published
tags:
- Company
- Database
- Event Sourcing
- Event Streaming
- Event Driven Architecture
- CQRS
- Data Infrastructure
- Developer Tools
- Cloud
- Open Source
- gRPC
- Agentic AI
trust_url: https://trust.kurrent.io/
---
