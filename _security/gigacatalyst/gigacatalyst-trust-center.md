---
certifications: []
description: ''
kind: trust-center
layout: security
name: Gigacatalyst Trust Center
name_suffix: Trust Center
overview: Gigacatalyst maintains a public trust center covering its security and compliance posture.
provider_name: Gigacatalyst
provider_slug: gigacatalyst
slug: gigacatalyst-trust-center
source_filename: gigacatalyst-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nsource: https://gigacatalyst.com/trust\nurl: https://gigacatalyst.com/trust\n# CORRECTION 2026-08-14: the mechanical probe extracted \"SOC 2\" from the page body\n# and recorded it as a held certification. It is not one. The trust center's own FAQ\n# reads: \"Do you have SOC 2? We are actively pursuing SOC 2 certification.\" Recording\n# it under certifications[] would credit Gigacatalyst with an attestation it does not\n# hold, so certifications[] is empty and the claim is carried under certifications_pursued[].\ncertifications: []\ncertifications_pursued:\n- name: SOC 2\n  status: pursuing\n  evidence: >-\n    https://gigacatalyst.com/trust FAQ - \"Do you have SOC 2? We are actively pursuing\n    SOC 2 certification. Our architecture is designed so that your customer data never\n    enters our systems, limiting exposure far beyond what a certification alone provides.\"\nposture:\n  summary: >-\n    Gigacatalyst publishes\
  \ a real trust center rather than a certification badge wall.\n    Its argument is architectural: generated apps run inside the customer's environment\n    under the signed-in user's own session credentials, so customer data is claimed never\n    to enter Gigacatalyst systems.\n  data_retention:\n    ai_providers: zero-retention\n    byok: true\n    stored:\n    - generated app source code\n    - app metadata (who created it, when)\n    - usage logs (optional, can be disabled)\n    never_stored:\n    - customer data or API responses\n    - query results or database contents\n    - end-user PII from the host platform\n    - AI prompts or responses\n  deployment_modes:\n  - mode: managed\n    default: true\n    description: >-\n      Requests route through the Gigacatalyst proxy for caching, rate limiting, and\n      analytics; AI powered by AWS Bedrock in the Gigacatalyst account (zero data\n      retention); basic telemetry via PostHog.\n  - mode: direct\n    default: false\n    description:\
  \ >-\n      API calls go straight to the customer's infrastructure with nothing routed through\n      Gigacatalyst; bring-your-own AI key (Vertex, Azure, AWS, or any provider); all\n      telemetry disabled.\n  write_access: >-\n    Granular and customer-selected - no writes, writes via the customer's existing API\n    endpoints, or new write operations through a Gigacatalyst intermediary. Destructive\n    endpoints can be disabled entirely.\n  breach_notification: within 24 hours of discovery, in writing\n  dpa: available on request via legal contact on the trust center\nsub_processors:\n- name: Supabase\n  purpose: App metadata storage\n  location: United States\n- name: Vercel\n  purpose: Hosting & deployment\n  location: United States\n- name: AWS Bedrock\n  purpose: AI code generation (default provider)\n  location: United States\n- name: PostHog\n  purpose: Product analytics (can be disabled)\n  location: United States\ndocuments:\n- title: Vulnerability Disclosure Policy\n  url:\
  \ https://gigacatalyst.com/trust/vulnerability-disclosure\n- title: Privacy Policy\n  url: https://gigacatalyst.com/privacy-policy\n- title: Terms of Service\n  url: https://gigacatalyst.com/terms-of-service\nevidence:\n- source: https://gigacatalyst.com/trust\n  http_status: 200\n  fetched: '2026-08-14'\n  keywords:\n  - soc 2\n  - trust center\n  - sub-processors\n  - breach notification\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gigacatalyst/refs/heads/main/security/gigacatalyst-trust-center.yml
summary_line: trust center published
tags:
- Company
- Artificial Intelligence
- Software-as-a-Service
- Sales Enablement
- Solutions Engineering
- Customer Success
- Automation
- No-Code
- Agents
- Embedded Analytics
- Low-Code
- Developer Tools
- Y Combinator
trust_url: https://gigacatalyst.com/trust
---
