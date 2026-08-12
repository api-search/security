---
api_specs:
- filename: openapi-public.json
  format: json
  label: Infer Responses API
  slug: infer-responses-api
  spec_type: OpenAPI
  url: https://infer.flow7.org/openapi-public.json
certifications: []
description: Infer publishes no trust center and holds no named third-party certification. It does publish a complete, versioned legal and data-protection document set, which is the closest thing it has to a trust surface. Recorded so the absence is a checked fact rather than an unchecked one.
kind: trust-center
layout: security
name: Infer By Flow7 Trust Center
name_suffix: Trust Center
overview: Infer by Flow7 maintains a public trust center covering its security and compliance posture.
provider_name: Infer by Flow7
provider_slug: infer-by-flow7
slug: infer-by-flow7-trust-center
source_filename: infer-by-flow7-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: >-\n  Probed https://infer.flow7.org/security (404) and reviewed every legal document linked from\n  https://infer.flow7.org/terms on 2026-08-11.\ndescription: >-\n  Infer publishes no trust center and holds no named third-party certification. It does publish a\n  complete, versioned legal and data-protection document set, which is the closest thing it has to a\n  trust surface. Recorded so the absence is a checked fact rather than an unchecked one.\ntrust_center: null\ntrust_center_probes:\n  - url: https://infer.flow7.org/security\n    status: 404\n  - url: https://infer.flow7.org/.well-known/security.txt\n    status: 404\ncertifications: []\ncertification_count: 0\nsoc2: false\niso27001: false\npci_dss: false\nhipaa: false\nfedramp: false\nnotes:\n  - HIPAA is explicitly out of scope — the Terms prohibit submitting protected health information.\n  - >-\n    PCI DSS is out of scope by architecture: Stripe-hosted Checkout\
  \ with Sold through Link, LLC as\n    merchant of record, and the Terms state Infer does not intentionally receive or store full card\n    numbers or card security codes.\n  - >-\n    The product was days old at probe time (all six Route Notes and every legal version date fall in\n    August 2026), so the absence of an audit report is expected rather than anomalous.\npublished_documents:\n  - name: Data Processing Addendum\n    url: https://infer.flow7.org/dpa\n    version: '2026-08-08'\n    regimes: [GDPR, UK GDPR, Swiss FADP, CCPA/CPRA and other US state privacy laws]\n  - name: Subprocessor Notice\n    url: https://infer.flow7.org/subprocessors\n    version: '2026-08-08'\n    note: Names six subprocessors by legal entity with role, data categories and location.\n  - name: Privacy Notice\n    url: https://infer.flow7.org/privacy\n    note: Section 9 lists security controls in prose.\n  - name: Acceptable Use Policy\n    url: https://infer.flow7.org/acceptable-use\n  - name: Legal Operator\
  \ Notice\n    url: https://infer.flow7.org/legal-operator\n  - name: Terms of Service\n    url: https://infer.flow7.org/terms\n  - name: Refund Policy\n    url: https://infer.flow7.org/refunds\n    version: '2026-08-08'\ndata_handling_commitments:\n  privacy_modes: [standard, no-training, zero-retention]\n  privacy_mode_source: RelayRequestOptions.privacy in openapi/infer-by-flow7-public-api-openapi.yml\n  note: >-\n    A per-request privacy mode is part of the wire contract, not just a policy page. Route eligibility\n    depends on it, and per-tier privacy_modes are published in the unauthenticated catalog. At probe\n    time (2026-08-11) all 66 callable tiers listed exactly [\"standard\"] and the 17 unavailable\n    :official tiers listed none — so no-training and zero-retention are contract-supported but not\n    currently offered on any published selector.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infer-by-flow7/refs/heads/main/security/infer-by-flow7-trust-center.yml
summary_line: trust center published
tags:
- AI/ML inference
- LLM API gateway
- Responses-compatible API
- Coding-agent tooling
- Developer tools
- Usage-based billing
- Prepaid billing
- Agent-native
- Agent Skills
- Model routing
trust_url: ''
---
