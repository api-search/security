---
api_specs:
- filename: typesafe-ai-openapi.yml
  format: yaml
  label: TypeSafe System One API
  slug: system-one-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typesafe-ai/refs/heads/main/openapi/typesafe-ai-openapi.yml
certification_count: 3
certifications:
- observed
- observed_note
- how_to_close
description: ''
kind: trust-center
layout: security
name: Typesafe Ai Trust Center
name_suffix: Trust Center
overview: TypeSafe AI maintains a public trust center documenting observed, observed_note, and how_to_close compliance.
provider_name: TypeSafe AI
provider_slug: typesafe-ai
slug: typesafe-ai-trust-center
source_filename: typesafe-ai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: https://trust.typesafe.ai/\nchecked: '2026-09-19'\nsummary: >-\n  TypeSafe runs a Vanta-hosted trust center at trust.typesafe.ai. It exists and it is the\n  authoritative location the Data Processing Agreement points at for the subprocessor list. Its\n  CONTENT could not be read: the page is a client-rendered Vanta application whose data API\n  (https://trust.typesafe.ai/graphql) rejects unsigned requests with \"Missing `signature` or\n  `signedAt`\". No certification is recorded here because none was observed.\npresent: true\nurl: https://trust.typesafe.ai/\nplatform: Vanta\nplatform_evidence:\n  - The served HTML loads only assets.vanta.com bundles (index-trust-report-*.js, alpaca-*.css).\n  - 'Vanta slug id on the <head> element: fa36t9a4dulcnactq79ryr.'\n  - 'Page <title>: \"Typesafe.ai Trust Center\"; canonical https://trust.typesafe.ai.'\nmachine_readable: false\nmachine_readable_note: >-\n  The trust report renders client-side.\
  \ Probed https://trust.typesafe.ai/graphql (400, \"Missing\n  `signature` or `signedAt`\"), https://api.vanta.com/graphql (410, retired in favour of the Vanta\n  REST API) and https://trust.typesafe.ai/api/graphql (404). Nothing on this host is fetchable by a\n  crawler or an agent.\ncertifications:\n  observed: []\n  observed_note: >-\n    DELIBERATELY EMPTY. A Vanta trust center usually lists SOC 2 / ISO 27001 status, but none was\n    visible in served HTML and the data API is signature-gated, so recording one would be a guess.\n    No `Compliance` pointer is emitted in apis.yml on the strength of an unreadable page — the\n    compliance_published check must read a genuine unknown here rather than credit an assumption.\n  how_to_close: >-\n    If TypeSafe (or a reader) can name the certifications the portal lists, this file and a\n    `Compliance` pointer can be filled in the same pass. Corrections are free — see README.\nsections_referenced_by_legal_documents:\n  - url: https://trust.typesafe.ai/subprocessors\n\
  \    named_by: 'Data Processing Agreement §3.1 (Authorization)'\n    quote: >-\n      \"Customer provides general authorization for Typesafe to engage the following subprocessors as\n      described in https://trust.typesafe.ai/subprocessors\"\n    probed: {url: 'https://trust.typesafe.ai/subprocessors', status: 200}\n    readable: false\n    readable_note: >-\n      Returns the same 6,914-byte Vanta shell as every other path on this host, so the subprocessor\n      table itself was NOT observed. The DPA clause is the substance; the table is not machine-readable.\nevidence:\n- url: https://trust.typesafe.ai/\n  status: 200\n  content_type: text/html\n  bytes: 6914\n- url: https://trust.typesafe.ai/subprocessors\n  status: 200\n  bytes: 6914\n- url: https://trust.typesafe.ai/graphql\n  status: 400\n  body: '{\"data\":null,\"errors\":[{\"message\":\"Missing `signature` or `signedAt`\", ... }]}'\n- url: https://typesafe.ai/trust\n  status: 404\ncross_links:\n  vulnerability_disclosure: security/typesafe-ai-vulnerability-disclosure.yml\n\
  \  regulatory: regulatory/typesafe-ai-regulatory-posture.yml\n  conformance: conformance/typesafe-ai-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/typesafe-ai/refs/heads/main/security/typesafe-ai-trust-center.yml
summary_line: observed, observed_note, how_to_close
tags:
- Artificial Intelligence
- Machine Learning
- Classification
- Content Moderation
- Decision Support
- Structured Outputs
- Inference
- LLM Alternative
- Agent Skills
- MCP
- Agent-Native
- Developer Tools
- A2A
trust_url: https://trust.typesafe.ai/
---
