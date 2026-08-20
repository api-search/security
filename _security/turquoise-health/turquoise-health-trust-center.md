---
api_specs:
- filename: turquoise-health-consumer-pricing-openapi.yml
  format: yaml
  label: Turquoise Consumer Pricing API
  slug: turquoise-consumer-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turquoise-health/refs/heads/main/openapi/turquoise-health-consumer-pricing-openapi.yml
certifications:
- SOC 2 Type II
- HIPAA
description: ''
kind: trust-center
layout: security
name: Turquoise Health Trust Center
name_suffix: Trust Center
overview: Turquoise Health maintains a public trust center documenting SOC 2 Type II and HIPAA compliance.
provider_name: Turquoise Health
provider_slug: turquoise-health
slug: turquoise-health-trust-center
source_filename: turquoise-health-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nurl: https://app.vanta.com/turquoise.health/trust/4eadhio8ef1h3zwumb77kp\nplatform: Vanta\nnote: >-\n  probe-security-programs.py returned trust=none because it only checks trust.<domain>,\n  security.<domain> and <domain>/trust|/security|/compliance — all of which 404 here.\n  Turquoise's trust center is hosted off-domain on Vanta, and the canonical link to it is\n  buried in the HIPAA compliance section of the Personalized Estimates developer doc rather\n  than in the site footer. Found by reading that doc.\n\nx-evidence:\n- fetched: '2026-08-14'\n  url: https://app.vanta.com/turquoise.health/trust/4eadhio8ef1h3zwumb77kp\n  http_status: 200\n  content_type: text/html\n  note: >-\n    Live and reachable, but a client-rendered single-page app — the certification list is\n    not present in the served HTML, so the certifications below are sourced from Turquoise's\n    own pages rather than scraped from the trust center\
  \ itself.\n- fetched: '2026-08-14'\n  url: https://turquoise.health/api/docs/personalized-estimates.md\n  http_status: 200\n  quote: >-\n    \"See our Trust Center for our current security certifications and compliance\n    documentation.\"\n- fetched: '2026-08-14'\n  url: https://turquoise.health/\n  http_status: 200\n  keywords: [SOC 2 Type II]\n- fetched: '2026-08-14'\n  url: https://turquoise.health/plans/providers\n  http_status: 200\n  keywords: [SOC 2 Type II, HIPAA]\n- fetched: '2026-08-14'\n  url: https://turquoise.health/platform\n  http_status: 200\n  keywords: [SOC 2 Type II, HIPAA]\n\ncertifications:\n- name: SOC 2 Type II\n  source: https://turquoise.health/plans/providers\n- name: HIPAA\n  source: https://turquoise.health/api/docs/personalized-estimates.md\n\nsafeguards:\n- Traffic to PHI-bearing endpoints routed to isolated environments subject to HIPAA\n  administrative, physical and technical safeguards.\n- PHI encrypted in transit and at rest.\n- Access to PHI logged\
  \ for audit purposes.\n- Production PHI access requires a signed Business Associate Agreement (BAA).\n- Demo environment does not accept live patient data; no PHI may be exchanged in it.\n\nenterprise_controls:\n- SSO (enterprise plans)\n- Granular permission controls\n- Audit logging\nsource_enterprise_controls: plans/turquoise-health-plans-pricing.yml\n\ngaps:\n- No /.well-known/security.txt on any host (RFC 9116).\n- No published vulnerability disclosure policy, responsible-disclosure page or bug bounty\n  program found; probe-security-programs.py returned vdp=none.\n- The trust center is not linked from the site footer or the docs navigation, only from\n  inside one developer doc.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turquoise-health/refs/heads/main/security/turquoise-health-trust-center.yml
summary_line: SOC 2 Type II, HIPAA
tags:
- Healthcare
- Price Transparency
- Hospital Rates
- Payer Rates
- Machine-Readable Files
- FHIR
- Health Insurance
- Negotiated Rates
- Out-of-Pocket Costs
- MRF
- Consumer Pricing
- MCP
- Eligibility
- Standard Service Packages
- HIPAA
trust_url: https://app.vanta.com/turquoise.health/trust/4eadhio8ef1h3zwumb77kp
---
