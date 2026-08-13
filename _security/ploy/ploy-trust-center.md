---
certifications:
- SOC 2 Type II
description: ''
kind: trust-center
layout: security
name: Ploy Trust Center
name_suffix: Trust Center
overview: Ploy maintains a public trust center documenting SOC 2 Type II compliance.
provider_name: Ploy
provider_slug: ploy
slug: ploy-trust-center
source_filename: ploy-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nprobe: true\nurl: https://trust.ploy.ai/\nstatus: 200\nchecked: '2026-08-12'\nplatform: Vanta\nplatform_evidence: >-\n  The page is served by Vanta (assets.vanta.com signature manifest, data-slugid\n  24unibf0zzlnq8wqjcyz) and is titled \"runploy.com Trust Center\" — runploy.com is\n  Ploy's other corporate domain, also used for support@runploy.com.\ncertifications:\n- name: SOC 2 Type II\n  status: claimed\n  evidence: >-\n    Listed as an Enterprise plan entitlement on https://ploy.ai/pricing (HTTP\n    200, read 2026-08-12) and linked from docs.ploy.ai/security as \"For\n    compliance documentation, security reports, and real-time subprocessor and\n    status information, visit our Trust Center.\"\n  report_access: request through the trust center\nnote: >-\n  The trust center body is rendered client-side, so the certification list could\n  not be read from the raw HTML — only the page's presence, platform and title\n  are recorded\
  \ as probed. The SOC 2 Type II claim is cited from Ploy's own\n  pricing page rather than from the trust center DOM, so it is marked `claimed`\n  rather than verified. The trust center advertises subprocessor and real-time\n  status information as well.\nevidence:\n- source: https://trust.ploy.ai/\n  status: 200\n  kind: trust center (Vanta-hosted)\n- source: https://ploy.ai/pricing\n  status: 200\n  kind: published SOC 2 Type II claim\n- source: https://docs.ploy.ai/security\n  status: 200\n  kind: security & compliance page linking the trust center\nsecurity_posture:\n  encryption_at_rest: AES-256\n  encryption_in_transit: HTTPS everywhere; ACME-provisioned certificates per custom domain\n  build_isolation: sandboxed per-build environments, no cross-workspace access\n  deploy_model: immutable snapshots with instant rollback\n  integration_auth: OAuth 2.0 with scoped permissions; no stored passwords\n  ai_training: workspace content is not used to train AI models\n  account_controls:\
  \ passkeys and SSO controls documented at https://docs.ploy.ai/enhanced-security\n  source: https://docs.ploy.ai/security\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ploy/refs/heads/main/security/ploy-trust-center.yml
summary_line: SOC 2 Type II
tags:
- Company
- Marketing
- Marketing Automation
- Artificial Intelligence
- AI Agents
- SEO
- Website Builder
- Growth
- Advertising
- Webhooks
- CLI
- Agent Skills
trust_url: https://trust.ploy.ai/
---
