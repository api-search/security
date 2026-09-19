---
certification_count: 2
certifications:
- SOC 2 Type II
- HIPAA
description: ''
kind: trust-center
layout: security
name: Aidora Trust Center
name_suffix: Trust Center
overview: Aidora maintains a public trust center documenting SOC 2 Type II and HIPAA compliance.
provider_name: Aidora
provider_slug: aidora
slug: aidora-trust-center
source_filename: aidora-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: https://trust.getaidora.com/\nnote: >-\n  Aidora runs a real, first-party trust center at trust.getaidora.com — a Vanta-hosted trust report\n  served from Aidora's own domain and branded \"Aidora Trust Center\". It is STILL LIVE (HTTP 200,\n  6,511 bytes) after the Paylocity acquisition, which makes it the only machine-addressable\n  compliance surface the company still serves. Its CONTENT, however, is not machine-readable: the\n  served HTML is a shell and the certification list loads client-side from a GraphQL endpoint that\n  requires a request signature (POST /graphql returns\n  {\"errors\":[{\"message\":\"Missing `signature` or `signedAt`\"}]}, HTTP 400). We did not attempt to\n  produce a signature. The certifications below are therefore recorded from Aidora's own published\n  security page, which is archived rather than live — see each entry's evidence.\ntrust_center:\n  url: https://trust.getaidora.com/\n  first_party:\
  \ true\n  host: trust.getaidora.com\n  platform: Vanta\n  title: Aidora Trust Center\n  status: 200\n  live: true\n  checked: '2026-09-14'\n  description: >-\n    \"At Aidora, we take the responsibility of handling sensitive data seriously. Our team is\n    committed to building secure systems, protecting privacy, and staying aligned with evolving\n    compliance standards.\" — og:description served by trust.getaidora.com.\n  machine_readable: false\n  machine_readable_note: >-\n    Vanta trust report SPA. Certification data is behind a signed GraphQL call, so no crawler or\n    agent can read the posture this page exists to publish.\ncertifications:\n- name: SOC 2 Type II\n  claimed: true\n  verified_live: false\n  evidence: https://web.archive.org/web/20260415000544/https://getaidora.com/security-standards\n  evidence_status: 200\n  evidence_kind: archived-first-party\n  quote: >-\n    \"We are SOC 2 Type II compliant, ensuring that we have state of the art security measures in\n   \
  \ place. The audit report can be accessed in our Trust Center.\"\n  note: >-\n    Aidora's own /security-standards page stated this. That page no longer exists — the live URL\n    now returns the acquisition-notice catch-all — so the claim is recorded from the 2026-04-15\n    archive snapshot and is NOT independently confirmed. The audit report itself was always gated\n    behind the trust center.\n- name: HIPAA\n  claimed: false\n  applicable: false\n  evidence: https://web.archive.org/web/20260415000544/https://getaidora.com/security-standards\n  evidence_status: 200\n  evidence_kind: archived-first-party\n  note: >-\n    Recorded because Aidora explicitly ANALYSED and DISCLAIMED it rather than ignoring it: the\n    company argued HIPAA does not apply, since PHI expressly excludes general HR data and\n    employer-held FMLA medical information. A deliberate, reasoned non-applicability, not a gap.\ncompliance_program:\n  monitoring_vendor: Vanta\n  monitoring_frequency: hourly automated\
  \ security and compliance checks\n  remediation_sla: high-priority findings resolved within 3 business days\n  evidence: https://web.archive.org/web/20260415000544/https://getaidora.com/security-standards\n  evidence_kind: archived-first-party\nsecurity_practices:\n  note: >-\n    Captured from Aidora's archived first-party security overview. Included because it is the only\n    substantive technical disclosure the company ever published, and because the platform choices\n    explain the absence of an API surface.\n  encryption_at_rest: AES-256\n  encryption_in_transit: TLS\n  waf: Cloudflare\n  hosting: Vercel (application), Supabase (database)\n  backups: continuous, with Point-In-Time Recovery\n  authentication: magic links and OAuth with major providers such as Google\n  personnel: background checks, annual security training, centrally managed encrypted laptops\n  ci_security: automated dependency vulnerability scanning, static analysis, OSS license scanning\n  evidence: https://web.archive.org/web/20260415000544/https://getaidora.com/security-standards\n\
  \  evidence_kind: archived-first-party\ngaps:\n- No /.well-known/security.txt on any Aidora host (probed 2026-09-14; see well-known/aidora-well-known.yml).\n- No published vulnerability disclosure policy or bug bounty program found.\n- The live security-standards page was removed at acquisition; only the trust center survived.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aidora/refs/heads/main/security/aidora-trust-center.yml
summary_line: SOC 2 Type II, HIPAA
tags:
- Company
- Human Resources
- Leave Management
- Absence Management
- HR Compliance
- Workforce
- Artificial Intelligence
- Software-as-a-Service
- Acquired
trust_url: ''
---
