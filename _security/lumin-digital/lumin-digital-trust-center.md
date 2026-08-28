---
certifications: []
description: ''
kind: trust-center
layout: security
name: Lumin Digital Trust Center
name_suffix: Trust Center
overview: Lumin Digital maintains a public trust center covering its security and compliance posture.
provider_name: Lumin Digital
provider_slug: lumin-digital
slug: lumin-digital-trust-center
source_filename: lumin-digital-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://trust.lumindigital.com/\nnote: >-\n  Lumin Digital operates a real, provider-served trust centre: trust.lumindigital.com is a CNAME to\n  lumindigital.trustshare.com (TrustShare, hosted on Render) and returns HTTP 200. Its contents are\n  NOT readable without executing JavaScript — the served HTML is a 29,173-byte Create React App shell\n  whose only asset is /static/index-BvjbS4dZ.js, and every path under the host returns that same\n  shell byte-for-byte. No certification names, audit reports, subprocessor list or document-request\n  flow could be enumerated from the served markup, so none are recorded here. The certifications\n  Lumin Digital does state publicly are captured in conformance/lumin-digital-conformance.yml from\n  the server-rendered https://lumindigital.com/security/ page.\ntrust_center:\n  url: https://trust.lumindigital.com/\n  status: 200\n  vendor: TrustShare\n  cname: lumindigital.trustshare.com\n\
  \  machine_readable: false\n  rendering: client-side SPA (Create React App shell)\n  certifications_enumerable: false\n  access: >-\n    The security page describes the GRC platform as \"client-accessible\", so the audit artifacts\n    behind it are expected to require an account or an NDA request.\ncertifications_named_elsewhere:\n- SOC 2 Trust Services Criteria\n- PCI Data Security Standard\n- GLBA-aligned security frameworks\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumin-digital/refs/heads/main/security/lumin-digital-trust-center.yml
summary_line: trust center published
tags:
- Digital Banking
- Banking
- Credit Unions
- Financial Services
- Fintech
- Core Banking
- Digital Account Opening
- Payments
- Commercial Banking
- SaaS
trust_url: ''
---
