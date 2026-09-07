---
api_specs:
- filename: yoodli-api-openapi.yml
  format: yaml
  label: Yoodli API
  slug: yoodli-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoodli/refs/heads/main/openapi/yoodli-api-openapi.yml
certification_count: 2
certifications:
- SOC 2 Type 2
- GDPR
description: ''
kind: trust-center
layout: security
name: Yoodli Trust Center
name_suffix: Trust Center
overview: Yoodli maintains a public trust center documenting SOC 2 Type 2 and GDPR compliance.
provider_name: Yoodli
provider_slug: yoodli
slug: yoodli-trust-center
source_filename: yoodli-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nprobe: true\nurl: https://trust.yoodli.ai/\nplatform: Vanta trust report\nlinked_from: https://yoodli.ai/ (homepage footer, twice)\ncertifications:\n- SOC 2 Type 2\n- GDPR\ncertifications_source: https://yoodli.ai/privacy\nevidence:\n- source: https://trust.yoodli.ai/\n  http_status: 200\n  bytes: 6378\n  keywords:\n  - Yoodli Trust Center\n  - vanta (x21)\n  note: 'Live and reachable, but client-rendered: the served HTML is a 6,378-byte Vanta shell that loads everything\n    from assets.vanta.com. No certification name, subprocessor list or security contact could be read from the response\n    body, so the certification list here is NOT taken from this page.'\n- source: https://yoodli.ai/privacy\n  http_status: 200\n  bytes: 172507\n  keywords:\n  - SOC2 (x4)\n  - SOC 2 Type 2\n  - GDPR\n  note: Yoodli's own privacy policy is server-rendered and names SOC 2 Type 2 and GDPR directly. This is the machine-readable\n    source for the\
  \ claim.\n- source: https://app.vanta.com/doc?s=ksgyk5j5biz8letqaidv4a\n  note: Document link embedded in the trust page shell; not fetched.\ngaps:\n- No ISO 27001, PCI DSS, HIPAA or FedRAMP claim was found on any server-rendered Yoodli page.\n- No security.txt on any host (/.well-known/security.txt returns 404 everywhere — see well-known/yoodli-well-known.yml).\n- 'No responsible-disclosure or vulnerability-disclosure page: /responsible-disclosure, /security/responsible-disclosure\n  and /vulnerability-disclosure all 404, and hackerone.com/yoodli and bugcrowd.com/yoodli both 404. No Security\n  pointer is emitted — there is no disclosure program to point at.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yoodli/refs/heads/main/security/yoodli-trust-center.yml
summary_line: SOC 2 Type 2, GDPR
tags:
- Artificial Intelligence
- Communication
- Coaching
- Learning and Development
- Sales Enablement
- Speech Analysis
- Human Resources
- Enterprise Software
- SaaS
- Identity Management
trust_url: https://trust.yoodli.ai/
---
