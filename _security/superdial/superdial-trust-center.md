---
api_specs:
- filename: superdial-api-openapi.yml
  format: yaml
  label: SuperDial API
  slug: superdial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superdial/refs/heads/main/openapi/superdial-api-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Superdial Trust Center
name_suffix: Trust Center
overview: SuperDial maintains a public trust center covering its security and compliance posture.
provider_name: SuperDial
provider_slug: superdial
slug: superdial-trust-center
source_filename: superdial-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://www.superdial.com/ (footer \"Security\" link)\npresent: true\nurl: https://app.vanta.com/thesuperbill.com/trust/yxpg5guedf5rle15cka4ab\nplatform: Vanta\nhttp_status: 200\nlinked_from: https://www.superdial.com/ footer, labelled \"Security\"\nmachine_readable: false\nreadable_by_crawler: false\nevidence:\n- {url: 'https://app.vanta.com/thesuperbill.com/trust/yxpg5guedf5rle15cka4ab', status: 200, note: '5,362-byte JavaScript shell; no certification names present in the served HTML'}\n- {url: 'https://www.superdial.com/security', status: 404}\n- {url: 'https://www.superdial.com/trust', status: 404}\ncertifications_claimed:\n- {name: HIPAA, source: SuperDial public statements and 2025 Series A press coverage}\n- {name: SOC 2 Type II, source: 'SuperDial public statements; audit reported completed November 2025'}\n- {name: HITRUST e1, source: SuperDial public statements}\npractices_claimed:\n- BAAs executed before PHI exchange\n\
  - AES-256 encryption at rest\n- TLS in transit for voice recordings, transcripts and extracted PHI\n- SSO and MFA\n- Customer-specific data controls, vendor security reviews\nnotes:\n- >-\n  A real, hosted trust center exists and is linked from the marketing footer — that part is\n  verified. What it lists could not be verified: the Vanta page renders entirely client-side, so a\n  crawler, an agent, or a procurement bot gets a 5KB empty shell.\n- >-\n  The trust center is registered under thesuperbill.com, the company's former name (SuperDial was\n  founded as SuperBill). A buyer verifying the vendor by domain will see a name that does not match\n  the product they are buying.\n- >-\n  SuperDial hosts no first-party security page at all — /security and /trust both 404 — so the\n  Vanta link is the only security surface, and its contents are unreadable to any non-browser\n  client.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superdial/refs/heads/main/security/superdial-trust-center.yml
summary_line: trust center published
tags:
- Company
- Healthcare
- Revenue Cycle Management
- Voice AI
- Insurance
- Artificial Intelligence
- Claims
- Prior Authorization
- Benefits Verification
- Automation
trust_url: https://app.vanta.com/thesuperbill.com/trust/yxpg5guedf5rle15cka4ab
---
