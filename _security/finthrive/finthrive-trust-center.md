---
certifications:
- SOC
- HITRUST
- NIST CSF
- EHNAC
description: ''
kind: trust-center
layout: security
name: Finthrive Trust Center
name_suffix: Trust Center
overview: FinThrive maintains a public trust center documenting SOC, HITRUST, NIST CSF, and EHNAC compliance.
provider_name: FinThrive
provider_slug: finthrive
slug: finthrive-trust-center
source_filename: finthrive-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nprobe: true\nsource: https://finthrive.com/security-and-data-trust-center\nurl: https://finthrive.com/security-and-data-trust-center\nnote: >-\n  The automated probe (0-working/probe-security-programs.py) missed this page because\n  FinThrive does not use any of the conventional locations — there is no trust.finthrive.com,\n  no security.finthrive.com, and no /trust, /security or /compliance path. The trust\n  center lives at the marketing-site slug /security-and-data-trust-center and was found\n  by reading the site's own sitemap.xml.\ncertifications:\n- SOC\n- HITRUST\n- NIST CSF\n- EHNAC\ncertification_notes: >-\n  The page states \"Strict Compliance with NIST CSF, HITRUST, SOC, EHNAC and industry\n  best practices\". It names \"SOC\" without qualifying the report type (SOC 1 vs SOC 2,\n  Type I vs Type II), so no more specific claim is recorded here. EHNAC is the\n  Electronic Healthcare Network Accreditation Commission, a healthcare-clearinghouse\n\
  \  accreditation specific to this sector.\ndocumentation_access:\n  portal: Whistic\n  gated: true\n  note: >-\n    Security documentation (SOC reports, HITRUST certification letters) is distributed\n    through a Whistic trust portal, which requires a request/NDA flow. The artifacts\n    themselves are not publicly downloadable.\nevidence:\n- source: https://finthrive.com/security-and-data-trust-center\n  http_status: 200\n  keywords: [NIST CSF, HITRUST, SOC, EHNAC, Whistic, trust center]\ngaps:\n- No /.well-known/security.txt on any FinThrive host (all 404 — see well-known/finthrive-well-known.yml).\n- No published vulnerability disclosure or bug bounty program, and no security@ contact\n  address stated on the trust center page.\n- No public status page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finthrive/refs/heads/main/security/finthrive-trust-center.yml
summary_line: SOC, HITRUST, NIST CSF, EHNAC
tags:
- Company
- Healthcare
- Revenue Cycle Management
- Health IT
- Claims
- Billing
- Payments
- Insurance
- Patient Access
- Analytics
- Software-as-a-Service
- United States
trust_url: https://finthrive.com/security-and-data-trust-center
---
