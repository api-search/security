---
api_specs:
- filename: cuein-answers-api-openapi.yml
  format: yaml
  label: Cuein answers API
  slug: cuein-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuein/refs/heads/main/openapi/cuein-answers-api-openapi.yml
- filename: cuein-conversations-api-openapi.yml
  format: yaml
  label: Cuein conversations API
  slug: cuein-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuein/refs/heads/main/openapi/cuein-conversations-api-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Cuein Trust Center
name_suffix: Trust Center
overview: Cuein maintains a public trust center covering its security and compliance posture.
provider_name: Cuein
provider_slug: cuein
slug: cuein-trust-center
source_filename: cuein-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nsource: https://cuein.ai/\nurl: https://app.vanta.com/cueinai/trust/7pzlr5lnec2vu3lghvusmd\nplatform: Vanta\ncertifications: []\nnote: >-\n  Cuein publishes a Vanta-hosted trust center, linked from the cuein.ai footer. The\n  page returns HTTP 200 but is a client-side application: the served HTML contains no\n  certification names, and a keyword scan of the response body for SOC 2, ISO 27001,\n  ISO 27017, ISO 27018, PCI DSS, HIPAA, FedRAMP, GDPR and CSA STAR returned zero\n  matches. The certification list exists only after script execution, so nothing is\n  asserted here and no Compliance pointer is emitted — the trust center's presence is\n  recorded, its contents are not claimed.\nevidence:\n  - source: https://cuein.ai/\n    kind: homepage-link\n    detail: footer \"Security\" link -> Vanta trust center\n  - source: https://app.vanta.com/cueinai/trust/7pzlr5lnec2vu3lghvusmd\n    kind: probe\n    http_status: 200\n\
  \    detail: JS-rendered; no certification string present in the served document\n    checked: '2026-08-14'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cuein/refs/heads/main/security/cuein-trust-center.yml
summary_line: trust center published
tags:
- Company
- Customer Experience
- Customer-Support
- Conversation Intelligence
- Generative AI
- Insights
- Knowledge Base
- Contact Center
trust_url: https://app.vanta.com/cueinai/trust/7pzlr5lnec2vu3lghvusmd
---
