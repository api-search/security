---
api_specs:
- filename: cogny-reports-api-openapi.yml
  format: yaml
  label: Cogny Reports API
  slug: cogny-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cogny/refs/heads/main/openapi/cogny-reports-api-openapi.yml
- filename: cogny-tickets-api-openapi.yml
  format: yaml
  label: Cogny Tickets API
  slug: cogny-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cogny/refs/heads/main/openapi/cogny-tickets-api-openapi.yml
- filename: cogny-warehouses-api-openapi.yml
  format: yaml
  label: Cogny Warehouses API
  slug: cogny-warehouses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cogny/refs/heads/main/openapi/cogny-warehouses-api-openapi.yml
- filename: cogny-webhooks-api-openapi.yml
  format: yaml
  label: Cogny Webhooks API
  slug: cogny-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cogny/refs/heads/main/openapi/cogny-webhooks-api-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Cogny Trust Center
name_suffix: Trust Center
overview: Cogny maintains a public trust center covering its security and compliance posture.
provider_name: Cogny
provider_slug: cogny
slug: cogny-trust-center
source_filename: cogny-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://cogny.com/security\nurl: https://cogny.com/security\nchecked: '2026-08-13'\nname: Cogny Security\ntype: security-page\nnote: >-\n  Cogny publishes a single self-hosted security page rather than a third-party\n  trust portal (no Vanta/Drata/SafeBase surface, no trust.cogny.com — probed,\n  404). The page is substantive: encryption posture, auth model, tenant\n  isolation, GDPR handling, infrastructure, a named sub-processor register, and\n  monitoring/incident response.\nattestation_correction: >-\n  IMPORTANT — a keyword probe of this page matches \"SOC 2\" and \"ISO 27001\", but\n  BOTH strings occur only inside the DeepInfra, Inc. row of the sub-processor\n  register (\"Zero data-retention policy; SOC 2 and ISO 27001 certified\"). They\n  describe a SUB-PROCESSOR, not Cogny AB. Cogny publishes no SOC 2 report, no\n  ISO 27001 certificate, and no PCI/HIPAA/FedRAMP claim anywhere on its public\n  surface. Recording\
  \ those certifications against Cogny would be a false\n  attribution, so they are held below under third_party_certifications only.\ncertifications: []\ncertifications_note: >-\n  None self-attested by Cogny AB as of the checked date.\ncompliance_programs:\n- id: gdpr\n  name: GDPR\n  status: claimed\n  self_attested: true\n  evidence: >-\n    Dedicated \"GDPR Compliance\" section — mandatory GDPR webhook endpoints\n    implemented for third-party integrations that require them (Shopify customer\n    data request, customer data erasure, shop data erasure); OAuth credentials\n    auto-deleted from the vault on integration disconnect; user-requested account\n    and warehouse deletion follow a scheduled confirm-then-purge process.\n  source: https://cogny.com/security\n- id: dpa\n  name: Data Processing Agreement\n  status: published\n  url: https://cogny.com/terms/dpa\n  http_status: 200\n  evidence: >-\n    Sub-processor contractual terms are set out in a published DPA linked from\n  \
  \  the security page.\n- id: dora\n  name: DORA addendum\n  status: published\n  url: https://cogny.com/terms/dora\n  http_status: 200\n  evidence: >-\n    A DORA (EU Digital Operational Resilience Act) addendum is published in the\n    terms set — relevant to EU financial-sector customers.\n- id: eu-data-residency\n  name: EU data residency\n  status: claimed\n  self_attested: true\n  evidence: >-\n    Compute on GKE europe-west1 (Belgium); Supabase managed Postgres on AWS\n    eu-north-1 (Stockholm); Berget AI for EU-hosted inference. The single stated\n    exception is Cogny Sites, which runs on Cloud Run in the customer's own GCP\n    project and region — EU, North American and Asian regions available, fixed at\n    creation.\n  source: https://cogny.com/security\n- id: ai-training-posture\n  name: AI training posture\n  status: claimed\n  self_attested: true\n  evidence: >-\n    Both Anthropic and OpenAI rows of the sub-processor register state the\n    provider \"does not train on\
  \ customer content submitted via the API\"; Hugging\n    Face \"does not store request bodies or responses when routing\"; DeepInfra\n    \"zero data-retention policy\".\n  source: https://cogny.com/security\nsecurity_controls:\n  encryption_in_transit: TLS (HTTPS) for all data, including service-to-service\n  encryption_at_rest: Supabase-encrypted database; OAuth tokens in Supabase Vault\n  authentication: Supabase Auth (email/password + social login)\n  third_party_oauth: OAuth 2.0 with HMAC signature verification on callbacks and webhooks\n  tenant_isolation: >-\n    Postgres Row-Level Security on all tables, scoped to the authenticated user's\n    warehouse; stated that cross-tenant access is not possible at the DB layer.\n  secret_handling: >-\n    Access and refresh tokens stored in Supabase Vault; stated never written to\n    application logs, client-side storage, or source code.\n  ddos_waf: Cloudflare edge CDN, WAF and DDoS mitigation in front of all public endpoints\n  ci_cd:\
  \ Google Cloud Build with container image scanning\n  monitoring: >-\n    Real-time monitoring of application errors, tool-execution failures and\n    security-relevant events, alerting engineering via Slack.\ndocuments:\n- name: Cogny Security Brief (PDF)\n  description: >-\n    A single vendor-review overview — company identity, data handling, storage\n    and retention, sub-processors, AI-training posture, and MCP connector\n    security. Offered as a download on the security page.\n  url: null\n  note: >-\n    No stable public PDF URL is exposed in the page markup (probed\n    /security-brief.pdf -> 404); the download appears to be generated or gated\n    behind the page. Recorded as published-but-not-directly-addressable.\nsub_processors:\n  register_published: true\n  source: https://cogny.com/security\n  count: 13\n  entries:\n  - name: Google Cloud (Google LLC / Google Cloud EMEA Ltd.)\n    purpose: Compute (GKE), BigQuery, object storage, build and deploy, Google-integration OAuth\n\
  \    location: europe-west1 (Belgium); hosted sites in customer-selected region\n  - name: Supabase, Inc.\n    purpose: Managed PostgreSQL, authentication, encrypted secret vault, point-in-time recovery\n    location: AWS eu-north-1 (Stockholm)\n  - name: Cloudflare, Inc.\n    purpose: Edge CDN, WAF, DDoS mitigation, TLS termination\n    location: Global edge\n    note: No personal data persisted at the edge\n  - name: Anthropic PBC\n    purpose: LLM inference (Claude) for AI reports and chat\n    location: Global routing\n  - name: OpenAI, L.L.C.\n    purpose: LLM inference (GPT models) for AI reports and chat\n    location: US + SCCs\n  - name: Berget AI\n    purpose: EU-hosted AI model inference\n    location: EU (Sweden)\n  - name: Hugging Face, Inc.\n    purpose: Inference routing for open-weights LLMs\n    location: US + SCCs\n  - name: DeepInfra, Inc.\n    purpose: LLM inference (DeepSeek open-weights) via Hugging Face routing\n    location: US + SCCs\n    third_party_certifications:\n\
  \    - SOC 2\n    - ISO 27001\n    note: >-\n      These certifications belong to DeepInfra, the sub-processor — NOT to Cogny.\n      See attestation_correction above.\n  - name: Brave Software, Inc. (Brave Search)\n    purpose: Web search, news, and rank-check data for AI research tools\n    location: US + SCCs\n  - name: Stripe Payments Europe, Ltd.\n    purpose: Subscription billing and payment processing\n    location: EU + SCCs\n  - name: Resend, Inc.\n    purpose: Transactional email (report and auth emails)\n    location: SCCs\n  - name: Slack Technologies, LLC\n    purpose: Internal alerting and optional customer notifications\n    location: SCCs\n  - name: ElevenLabs Inc.\n    purpose: Optional text-to-speech, invoked only when audio features are used\n    location: SCCs\nlegal_entity:\n  name: Cogny AB\n  address: Peter Myndes Backe 16, 118 46 Stockholm, Sweden\n  jurisdiction: SE\nrelated:\n- https://cogny.com/privacy\n- https://cogny.com/terms\n- https://cogny.com/terms/dpa\n\
  - https://cogny.com/terms/dora\n- https://cogny.com/cookies\nlast_updated_by_provider: 'March, 2026'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cogny/refs/heads/main/security/cogny-trust-center.yml
summary_line: trust center published
tags:
- Company
- Ai Enterprise Software
- Marketing
- Marketing Analytics
- Marketing Automation
- MCP
- Agents
- Data Warehouse
- Advertising
trust_url: https://cogny.com/security
---
