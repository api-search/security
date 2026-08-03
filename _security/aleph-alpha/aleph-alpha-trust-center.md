---
api_specs:
- filename: aleph-alpha-pharia-inference-openapi.json
  format: json
  label: PhariaInference API
  slug: pharia-inference
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleph-alpha/refs/heads/main/openapi/aleph-alpha-pharia-inference-openapi.json
- filename: aleph-alpha-pharia-data-openapi.json
  format: json
  label: PhariaData API
  slug: pharia-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleph-alpha/refs/heads/main/openapi/aleph-alpha-pharia-data-openapi.json
- filename: aleph-alpha-pharia-search-openapi.json
  format: json
  label: PhariaSearch / Document Index API
  slug: pharia-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleph-alpha/refs/heads/main/openapi/aleph-alpha-pharia-search-openapi.json
- filename: aleph-alpha-pharia-studio-openapi.json
  format: json
  label: PhariaStudio API
  slug: pharia-studio
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleph-alpha/refs/heads/main/openapi/aleph-alpha-pharia-studio-openapi.json
- filename: aleph-alpha-pharia-os-openapi.json
  format: json
  label: PhariaOS Manager API
  slug: pharia-os
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleph-alpha/refs/heads/main/openapi/aleph-alpha-pharia-os-openapi.json
- filename: aleph-alpha-responses-openapi.json
  format: json
  label: Responses API (Stateful Responses)
  slug: responses
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleph-alpha/refs/heads/main/openapi/aleph-alpha-responses-openapi.json
certifications: []
description: ''
kind: trust-center
layout: security
name: Aleph Alpha Trust Center
name_suffix: Trust Center
overview: Aleph Alpha maintains a public trust center covering its security and compliance posture.
provider_name: Aleph Alpha
provider_slug: aleph-alpha
slug: aleph-alpha-trust-center
source_filename: aleph-alpha-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nprobe: true\nurl: null\nnote: 'Aleph Alpha publishes no trust-center portal. trust.aleph-alpha.com and security.aleph-alpha.com\n  do not resolve, and /security, /trust and /compliance on aleph-alpha.com return 404 (probed\n  2026-08-02). Its published compliance posture lives in two places instead: an independently\n  listed ISO/IEC 27001:2022 certificate, and a supply-chain security disclosure page in the\n  installation guide.'\ncertifications:\n- standard: ISO/IEC 27001:2022\n  holder: Aleph Alpha GmbH\n  scope: 'Research, development and commercialization of generative AI technology with focus on multimodal large language models'\n  certificate_number: '31625355'\n  certifier: DQS\n  source: https://www.dqsglobal.com/en/customer-database/aleph-alpha-gmbh\nsupply_chain_security:\n  url: https://docs.aleph-alpha.com/phariaai-install-config-guide/latest/installation/before-you-start/security-disclosure-v2.html\n  practices:\n  -\
  \ 'Every PhariaAI container image cryptographically signed with Cosign keyless signing (GitHub Actions OIDC), bound to the exact image digest.'\n  - 'SLSA provenance verifiable with --verify.'\n  - 'CycloneDX SBOM attestation per image.'\n  - 'SPDX package and license metadata for compliance workflows.'\n  - 'Trivy build-time CVE findings published as a signed JSON attestation.'\n  - 'Verification scripts published at https://github.com/Aleph-Alpha/support (cosign-verify-image.sh, cosign-extract.sh).'\n  legacy: https://docs.aleph-alpha.com/phariaai-install-config-guide/latest/installation/before-you-start/security-disclosure-v1.html\n  purpose: 'Explicitly framed for archiving audit evidence for ISO 27001, SOC 2 and AIC4.'\nhosting_certifications:\n- standard: BSI C5, ISO 27001\n  holder: STACKIT GmbH (hosting provider for Pharia Government Assistant, Germany)\n  source: https://docs.aleph-alpha.com/verticals/pga-de/uebersicht.html\n  note: 'Provider-of-provider certification, not Aleph\
  \ Alpha''s own.'\nevidence:\n- {source: 'https://www.dqsglobal.com/en/customer-database/aleph-alpha-gmbh', kind: third-party-certificate-registry, keywords: ['ISO IEC 27001:2022']}\n- {source: 'https://docs.aleph-alpha.com/phariaai-install-config-guide/latest/installation/before-you-start/security-disclosure-v2.html', kind: docs, keywords: ['SBOM', 'SLSA', 'Cosign', 'ISO 27001', 'SOC 2', 'AIC4']}\nprobes:\n- {url: 'https://trust.aleph-alpha.com/', result: 'DNS does not resolve'}\n- {url: 'https://aleph-alpha.com/security/', http_status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aleph-alpha/refs/heads/main/security/aleph-alpha-trust-center.yml
summary_line: trust center published
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Large Language Models
- Generative AI
- Sovereign AI
- Inference
- Embeddings
- Semantic Search
- Vector Search
- Agents
- Model Context Protocol
- Germany
- Enterprise Software
- Government
trust_url: ''
---
