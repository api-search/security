---
api_specs:
- filename: hotel-engine-catalogservice-api-openapi.yml
  format: yaml
  label: Engine Catalog Service API
  slug: hotel-engine-catalogservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotel-engine/refs/heads/main/openapi/hotel-engine-catalogservice-api-openapi.yml
- filename: hotel-engine-contentservice-api-openapi.yml
  format: yaml
  label: Engine Content Service API
  slug: hotel-engine-contentservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotel-engine/refs/heads/main/openapi/hotel-engine-contentservice-api-openapi.yml
- filename: hotel-engine-lodgingbookingservice-api-openapi.yml
  format: yaml
  label: Engine Lodging Booking Service API
  slug: hotel-engine-lodgingbookingservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotel-engine/refs/heads/main/openapi/hotel-engine-lodgingbookingservice-api-openapi.yml
- filename: hotel-engine-lodgingshoppingservice-api-openapi.yml
  format: yaml
  label: Engine Lodging Shopping Service API
  slug: hotel-engine-lodgingshoppingservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotel-engine/refs/heads/main/openapi/hotel-engine-lodgingshoppingservice-api-openapi.yml
certifications:
- SOC 2 Type II
description: ''
kind: trust-center
layout: security
name: Hotel Engine Trust Center
name_suffix: Trust Center
overview: Engine maintains a public trust center documenting SOC 2 Type II compliance.
provider_name: Engine
provider_slug: hotel-engine
slug: hotel-engine-trust-center
source_filename: hotel-engine-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nprobe: true\nurl: https://trust.engine.com/\nsource: https://trust.engine.com/\nsummary: >-\n  Engine operates a hosted Trust Center at trust.engine.com, powered by Conveyor. The public\n  landing surface advertises SOC 2 Type II and GDPR/CCPA posture; the underlying evidence\n  documents are gated behind an NDA/access request, which is the normal Conveyor pattern.\nplatform: Conveyor\ncertifications:\n  - SOC 2 Type II\nprivacy_frameworks:\n  - GDPR\n  - CCPA\naccess: >-\n  Report and document downloads require requesting access through the Conveyor portal;\n  only the certification/framework badges are anonymously visible.\nevidence:\n  - source: https://trust.engine.com/\n    http_status: 200\n    page_title: Engine Trust Center | Powered by Conveyor\n    keywords: [soc2, 'SOC 2 Type II', gdpr, ccpa]\n    fetched: '2026-08-04'\nhosts_probed:\n  - {url: 'https://trust.engine.com', status: 200, result: trust-center}\n  - {url: 'https://security.engine.com',\
  \ status: null, result: no-dns}\n  - {url: 'https://www.engine.com/trust', status: 404}\n  - {url: 'https://www.engine.com/security', status: 404}\n  - {url: 'https://www.engine.com/compliance', status: 404}\nrelated:\n  vulnerability_disclosure: security/hotel-engine-vulnerability-disclosure.yml\n  domain_security: security/hotel-engine-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hotel-engine/refs/heads/main/security/hotel-engine-trust-center.yml
summary_line: SOC 2 Type II
tags:
- Company
- Travel
- Business Travel
- Lodging
- Hotels
- Booking
- Travel Management
- Expense Management
- Payments
- gRPC
- Protobuf
- Partner API
trust_url: https://trust.engine.com/
---
