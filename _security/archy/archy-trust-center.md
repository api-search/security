---
certifications:
- HIPAA
- ISO 9001
- SSAE 18
description: ''
kind: trust-center
layout: security
name: Archy Trust Center
name_suffix: Trust Center
overview: Archy maintains a public trust center documenting HIPAA, ISO 9001, and SSAE 18 compliance.
provider_name: Archy
provider_slug: archy
slug: archy-trust-center
source_filename: archy-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nprobe: false\nsource: https://trust.archy.com/\nurl: https://trust.archy.com/\nplatform: Vanta\n# Vanta-hosted trust center (SPA served from api.vanta.com; slug v4zuh4uom17th9wk5mociz).\n# The public trust page requires an in-app session to render the document/subprocessor\n# list, so certifications below are the ones Archy publishes on its own marketing surface\n# and are corroborated by third-party listings. No SOC 2 report was verifiable from a\n# public source at probe time.\ncertifications:\n- id: hipaa\n  name: HIPAA\n  status: compliant\n  evidence: https://www.archy.com/cloud-benefits\n  note: >-\n    \"Archy uses HIPAA-compliant Amazon Web Services based infrastructure that ensures a\n    high standard of data security and compliance with HIPAA.\" Corroborated across\n    third-party software directories.\n- id: iso-9001\n  name: ISO 9001\n  status: claimed\n  evidence: https://www.archy.com/cloud-benefits\n  note: >-\n  \
  \  Vendor-stated: \"Archy ensures top-tier protection with ISO 9001 and SSAE 18\n    certifications.\" Reads as infrastructure/AWS-level assurance; not independently verified.\n- id: ssae-18\n  name: SSAE 18\n  status: claimed\n  evidence: https://www.archy.com/cloud-benefits\n  note: Vendor-stated alongside ISO 9001; not independently verified.\nsecurity_contact: security@archy.com   # published in archy.com DNS CAA iodef record\nnotes:\n- Healthcare data (PHI) practice-management SaaS; HIPAA is the primary published posture.\n- No public developer/API surface; the Master Service Agreement restricts access to non-public APIs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archy/refs/heads/main/security/archy-trust-center.yml
summary_line: HIPAA, ISO 9001, SSAE 18
tags:
- Company
- Dental
- Healthcare
- Practice Management
- Dental Software
- SaaS
- Artificial Intelligence
- Payments
- Insurance
trust_url: https://trust.archy.com/
---
