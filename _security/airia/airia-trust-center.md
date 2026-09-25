---
api_specs:
- filename: airia-openapi.yml
  format: yaml
  label: Airia Web APIs
  slug: airia-web-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airia/refs/heads/main/openapi/airia-openapi.yml
certification_count: 0
certifications: []
description: 'Airia publishes a trust center at https://trust.airia.com/ (HTTP 200), hosted on Vanta — the page declares a canonical of https://trust.airia.com, loads assets.vanta.com bundles and links a Vanta document share (app.vanta.com/doc?s=...). The page is rendered entirely client-side: the HTML payload contains no certification names, no report list and no subprocessor table, and the Vanta trust-report API returns 401 to an anonymous caller. So the PORTAL is verified and the CONTENTS are not. No certification is recorded here, because none could be read without executing the page''s JavaScript, and an assumed SOC 2 would be an invention.'
kind: trust-center
layout: security
name: Airia Trust Center
name_suffix: Trust Center
overview: Airia maintains a public trust center covering its security and compliance posture.
provider_name: Airia
provider_slug: airia
slug: airia-trust-center
source_filename: airia-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: https://trust.airia.com/\ndescription: >-\n  Airia publishes a trust center at https://trust.airia.com/ (HTTP 200), hosted on Vanta — the page\n  declares a canonical of https://trust.airia.com, loads assets.vanta.com bundles and links a Vanta\n  document share (app.vanta.com/doc?s=...). The page is rendered entirely client-side: the HTML\n  payload contains no certification names, no report list and no subprocessor table, and the Vanta\n  trust-report API returns 401 to an anonymous caller. So the PORTAL is verified and the CONTENTS\n  are not. No certification is recorded here, because none could be read without executing the\n  page's JavaScript, and an assumed SOC 2 would be an invention.\ntrust_center:\n  url: https://trust.airia.com/\n  platform: Vanta\n  http_status: 200\n  content_readable: false\n  reason: js-rendered\n  document_share: https://app.vanta.com/doc?s=61f32r7tmxevtmh7apswt\n  certifications_named: []\n \
  \ subprocessors_published: unknown\n  checked: '2026-09-19'\nrelated_public_signals:\n- claim: GDPR and HIPAA\n  where: https://airia.com/ai-platform/security/\n  note: >-\n    Stated as regulatory standards the PLATFORM helps a customer meet (\"built-in policy enforcement\n    and automated reporting\"), not as an Airia attestation. Not counted as a compliance claim.\n- claim: 'SOC 2, ISO 27001, EU AI Act'\n  where: https://airia.com/llms.txt (Compliance Reporting page description)\n  note: Describes audit-ready reports the product generates for the customer, again not Airia's own certificates.\nvulnerability_disclosure:\n  published: false\n  probes:\n  - url: https://airia.com/.well-known/security.txt\n    status: 404\n  - url: https://airia.ai/.well-known/security.txt\n    status: 401\n  - url: https://api.airia.ai/.well-known/security.txt\n    status: 401\n  - url: https://airia.com/security\n    status: 404\n  note: >-\n    No security.txt, no published disclosure policy page and\
  \ no bug-bounty programme (HackerOne,\n    Bugcrowd, Intigriti) was found. A security researcher's only documented route is the general\n    contact form. No `Security` pointer is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airia/refs/heads/main/security/airia-trust-center.yml
summary_line: trust center published
tags:
- Company
- Enterprise AI
- AI Agents
- AI Governance
- AI Security
- MCP
- MCP Gateway
- Agent Orchestration
- LLM Gateway
- AI Discovery
- Red Teaming
- Guardrails
- Knowledge Retrieval
- RAG
- Agent-Native
trust_url: ''
---
