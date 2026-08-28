---
api_specs:
- filename: scale-computing-fleet-manager-openapi.json
  format: json
  label: SC//Fleet Manager API
  slug: scfleet-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-fleet-manager-openapi.json
- filename: scale-computing-core-openapi.json
  format: json
  label: Scale Computing Platform Core API
  slug: scale-computing-platform-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-core-openapi.json
certifications: []
description: ''
kind: trust-center
layout: security
name: Scale Computing Trust Center
name_suffix: Trust Center
overview: Scale Computing maintains a public trust center covering its security and compliance posture.
provider_name: Scale Computing
provider_slug: scale-computing
slug: scale-computing-trust-center
source_filename: scale-computing-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://www.scalecomputing.com/security\ntrust_center:\n  published: false\n  url: null\n  note: >-\n    No trust center found. trust.scalecomputing.com does not serve a page (Cloudflare edge answers the\n    hostname with a challenge to a raw client and returns HTTP 404 to a browser-agent fetch), and\n    www.scalecomputing.com/security is a product-marketing page, not a compliance portal.\ncertifications: []\nx-false-positive-correction:\n  detected_by: 0-working/probe-security-programs.py\n  detected: [SOC 2, PCI DSS]\n  verdict: rejected\n  reason: >-\n    The keyword probe matched \"SOC 2\" and \"PCI DSS\" on https://www.scalecomputing.com/security, but on\n    reading the page those strings appear in offerings Scale Computing sells TO customers (\"PCI DSS\n    Compliance Solutions for Secure, Scalable Payment Environments\", a free PCI assessment tool, and a\n    white paper titled \"Enabling Regulatory Compliance with\
  \ Your IT Infrastructure Platform\"). The page\n    makes no claim that Scale Computing itself holds a SOC 2 attestation or a PCI DSS certification, and\n    no such claim was found elsewhere on the site. Recorded as absent rather than credited.\n  checked: '2026-08-26'\nevidence:\n- url: https://www.scalecomputing.com/security\n  status: 200\n  finding: marketing page; compliance offerings for customers, no self-attestation\n- url: https://trust.scalecomputing.com\n  status: 404\n  finding: no trust center served (403 Cloudflare challenge to curl, 404 to a browser-agent fetch)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/security/scale-computing-trust-center.yml
summary_line: trust center published
tags:
- Edge Computing
- Hyperconverged Infrastructure
- Virtualization
- Infrastructure Management
- Fleet Management
- Virtual Machines
- Observability
- Infrastructure as Code
- Kubernetes
- Company
trust_url: ''
---
