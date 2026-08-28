---
certifications: []
description: ''
kind: trust-center
layout: security
name: Scaled Cognition Trust Center
name_suffix: Trust Center
overview: Scaled Cognition maintains a public trust center covering its security and compliance posture.
provider_name: Scaled Cognition
provider_slug: scaled-cognition
slug: scaled-cognition-trust-center
source_filename: scaled-cognition-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://trust.scaledcognition.com\ntrust_center:\n  present: true\n  url: https://trust.scaledcognition.com\n  http_status: 200\n  platform: Vanta Trust Center\n  ownership_evidence: >-\n    trust.scaledcognition.com is a CNAME to 66a3c59c17f6ad4ce8f7f32b.cname.vantatrust.com, a\n    per-tenant Vanta record published under a domain Scaled Cognition controls.\n  linked_from_site: false\n  linked_from_site_note: >-\n    The footer on scaledcognition.com carries a \"Trust Center\" item, but its anchor is href=\"#\" and\n    it is styled with the class \"hide\" — the trust center is live and unlinked.\n  certifications:\n  - name: SOC 2 Type II\n    source: https://www.scaledcognition.com/ai-info\n    verified: provider-published claim on the company's own AI-info page\n  certifications_note: >-\n    The Vanta page renders entirely client-side (a 5.5KB shell that loads\n    index-trust-report-*.js), so its certification list, subprocessors\
  \ and document-request flow\n    cannot be enumerated without executing JavaScript. The served HTML additionally carries a\n    cached canonical/meta block belonging to a different Vanta tenant, which is a Vanta shared-shell\n    artifact and NOT evidence about Scaled Cognition — no certification was read from it.\n  security_contact: hello@scaledcognition.com\n  security_contact_source: https://www.scaledcognition.com/contact\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scaled-cognition/refs/heads/main/security/scaled-cognition-trust-center.yml
summary_line: trust center published
tags:
- Artificial Intelligence
- Agents
- Large Language Models
- Customer Experience
- Contact Center
- Conversational AI
- Voice
- Enterprise Software
- Machine Learning
- Company
trust_url: ''
---
