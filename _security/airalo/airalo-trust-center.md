---
api_specs:
- filename: airalo-partner-api-openapi.yml
  format: yaml
  label: Airalo Partner API
  slug: airalo-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airalo/refs/heads/main/openapi/airalo-partner-api-openapi.yml
certification_count: 0
certifications: []
description: ''
kind: trust-center
layout: security
name: Airalo Trust Center
name_suffix: Trust Center
overview: Airalo maintains a public trust center covering its security and compliance posture.
provider_name: Airalo
provider_slug: airalo
slug: airalo-trust-center
source_filename: airalo-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nprobe: true\nurl: https://trust.airalo.com\nplatform: Vanta\ncertifications: []\nevidence:\n- source: https://trust.airalo.com\n  http_status: 200\n  fetched: '2026-09-19'\n  keywords: [trust center, security, compliance]\n  note: >-\n    First-party host serving a Vanta trust center. The page title is \"Airalo Trust Center\" and its meta\n    description states Airalo has \"built a robust foundation of security and transparency\". The report body\n    is entirely client-rendered; the underlying data endpoint (trust.airalo.com/graphql) rejects anonymous\n    requests with \"Missing `signature` or `signedAt`\", and the linked control document\n    (app.eu.vanta.com/doc?s=...) returns an image rather than readable text.\n- source: https://www.airalo.com/.well-known/security.txt\n  http_status: 404\n  note: No RFC 9116 security.txt on any Airalo host.\nnote: >-\n  The trust center exists and is first-party, but NO named certification\
  \ (SOC 2, ISO 27001, PCI DSS, HIPAA,\n  FedRAMP) could be verified from a public surface, so none is claimed here and no Compliance pointer is\n  emitted. A reader should open trust.airalo.com in a browser to see the current control set.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airalo/refs/heads/main/security/airalo-trust-center.yml
summary_line: trust center published
tags:
- Company
- eSIM
- Telecommunications
- Travel
- Connectivity
- Mobile Data
- Roaming
- Partner API
- Webhook
- Singapore
trust_url: https://trust.airalo.com
---
