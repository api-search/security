---
certifications:
- ISO 27001
- SOC 2 Type II
description: ''
kind: trust-center
layout: security
name: Levity Trust Center
name_suffix: Trust Center
overview: Levity maintains a public trust center documenting ISO 27001 and SOC 2 Type II compliance.
provider_name: Levity
provider_slug: levity
slug: levity-trust-center
source_filename: levity-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nurl: https://trust.levity.ai/\nplatform: Vanta\ncertifications:\n- name: ISO 27001\n  status: certified\n  source: https://levity.ai/en/security\n- name: SOC 2 Type II\n  status: certified\n  report_access: available on request via the Trust Center\n  source: https://levity.ai/en/security\ncompliance:\n- name: GDPR\n  status: compliant\n  source: https://levity.ai/en/security\n- name: DPA\n  status: published\n  url: https://levity.ai/en/legal/dpa\nnot_claimed:\n- HIPAA\n- PCI DSS\n- FedRAMP\n- ISO 27017\n- ISO 27018\nsecurity_posture:\n  infrastructure: private clouds on AWS, Google Cloud and Microsoft Azure\n  encryption: HTTPS for all network interactions; sensitive data encrypted in transit\n    and at rest\n  authentication: delegated to WorkOS (Levity does not store passwords)\n  payments: handled by third-party processors (Stripe, Paddle); Levity stores no payment\n    information\n  source: https://levity.ai/en/security\n\
  evidence:\n- source: https://trust.levity.ai/\n  status: 200\n  kind: trust-center\n  detail: Live Vanta-hosted Trust Center (content rendered client-side; the certification\n    list below is taken from the linked security page rather than scraped from the\n    Vanta shell).\n- source: https://levity.ai/en/security\n  status: 200\n  kind: security-page\n  keywords: [iso 27001, soc 2 type ii, gdpr, trust center]\nnotes:\n- No subprocessor list was found at a public URL (/en/legal/sub-processors was not\n  resolvable); subprocessors are presumably disclosed inside the Vanta Trust Center\n  after access request.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/levity/refs/heads/main/security/levity-trust-center.yml
summary_line: ISO 27001, SOC 2 Type II
tags:
- Company
- Artificial Intelligence
- Logistics
- Supply Chain
- Freight
- Workflow Automation
- Email
- Document Processing
- SaaS
trust_url: https://trust.levity.ai/
---
