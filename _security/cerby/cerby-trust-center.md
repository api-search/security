---
certifications: []
description: ''
kind: trust-center
layout: security
name: Cerby Trust Center
name_suffix: Trust Center
overview: Cerby maintains a public trust center covering its security and compliance posture.
provider_name: Cerby
provider_slug: cerby
slug: cerby-trust-center
source_filename: cerby-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nprobe: true\nurl: https://trust.cerby.com/\nexists: true\ncontents_readable: false\nplatform: Drata\nplatform_evidence:\n  dns: trust.cerby.com CNAME trust.cname.drata.com\n  detail: >-\n    trust.cerby.com is a genuinely provisioned host, not the *.cerby.com\n    wildcard. Control probe: zzznotreal.cerby.com returns HTTP 200 from an AWS\n    origin identifying itself as \"server: banana\", while trust.cerby.com returns\n    HTTP 403 from Cloudflare with a challenge ray and CNAMEs to Drata's trust\n    center service. Different origin, different response — the trust center is\n    real.\naccess:\n  http_status: 403\n  reason: Cloudflare interactive bot challenge (\"Just a moment... Enable JavaScript and cookies to continue\")\n  browser_ua_retried: true\n  outcome: >-\n    The certification list could not be read. Cerby's own attestations, if any,\n    live behind this challenge.\ncertifications: []\ncertifications_note: >-\n  DELIBERATELY\
  \ EMPTY. No certification is attributed to Cerby because none could\n  be verified. This is the trap on this provider and it is worth stating plainly:\n  https://www.cerby.com/security returns 200 and does name SOC 2 Type I, SOC 2\n  Type II and ISO 27001 — but its section 1 is titled \"CLOUD PROVIDER's Audits &\n  Certifications\", and section 1.1 reads \"Cerby currently relies on its Cloud\n  Provider's third-party reviewed Security Program\". Section 1.3 goes further:\n  \"To the extent Cerby does not obtain a Third-Party Audit of its own, Cerby will\n  adopt or maintain ... an equivalent, industry-recognized framework\" — the\n  document explicitly contemplates Cerby having no audit of its own. Harvesting\n  those certification names would attribute a subprocessor's attestations to\n  Cerby. They are recorded below as what they are.\ncloud_provider_requirements_published:\n  relied_on_by_cerby: [SOC 2 Type I]\n  required_of_cloud_providers: [SOC 2 Type II, ISO 27001]\n  attributed_to:\
  \ Cerby's cloud provider, NOT Cerby\n  source: https://www.cerby.com/security\nsecurity_policy:\n  url: https://www.cerby.com/security\n  title: Security Policy | Cerby\n  type: contractual security addendum\n  http_status: 200\n  published_commitments:\n  - Customer Data encrypted at rest with AES 256-bit or better.\n  - TLS 1.2 or better for Customer Data in transit over untrusted networks.\n  - Encryption keys logically separated from Customer Data.\n  - Customer Data hosted in the United States production cloud environment, or another mutually agreed region.\n  - Critical and high vulnerabilities addressed within 30 days, medium within 90 days, on commercially reasonable efforts.\nx-evidence:\n- url: https://trust.cerby.com/\n  http_status: 403\n  fetched: '2026-08-09'\n- url: https://www.cerby.com/security\n  http_status: 200\n  fetched: '2026-08-09'\n- url: https://zzznotreal.cerby.com/\n  http_status: 200\n  fetched: '2026-08-09'\n  role: false-positive control\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerby/refs/heads/main/security/cerby-trust-center.yml
summary_line: trust center published
tags:
- Identity
- Access Management
- Security
- Password Management
- Provisioning
- SCIM
- Identity Governance
- Nonfederated Applications
- Automation
- Webhooks
trust_url: https://trust.cerby.com/
---
