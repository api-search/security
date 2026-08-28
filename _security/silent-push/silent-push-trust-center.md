---
api_specs:
- filename: silent-push-web-scanner.postman_collection.json
  format: json
  label: Silent Push API
  slug: silent-push-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/silent-push/refs/heads/main/postman/silent-push-web-scanner.postman_collection.json
certifications: []
description: ''
kind: trust-center
layout: security
name: Silent Push Trust Center
name_suffix: Trust Center
overview: Silent Push maintains a public trust center covering its security and compliance posture.
provider_name: Silent Push
provider_slug: silent-push
slug: silent-push-trust-center
source_filename: silent-push-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: >-\n  direct probes of trust.silentpush.com, www.silentpush.com/trust/,\n  www.silentpush.com/security/, www.silentpush.com/legal/, plus keyword scans of\n  the terms of use and privacy policy\ntrust_center:\n  published: false\ncertifications: []\ncompliance_programs: []\nnote: >-\n  No trust center exists. trust.silentpush.com does not resolve;\n  www.silentpush.com/trust/, /security/ and /legal/ all return 404. Scanning the\n  published Terms of Use and Privacy Policy for SOC 2, ISO 27001, PCI DSS,\n  HIPAA, FedRAMP, GDPR and CCPA returned no match, so no compliance posture is\n  publicly claimed and NO Compliance pointer is emitted. Silent Push does\n  publish a vulnerability disclosure policy - see\n  security/silent-push-vulnerability-disclosure.yml.\nx-evidence:\n- url: https://trust.silentpush.com/\n  http_status: '<no response - DNS did not resolve>'\n  fetched: '2026-08-27'\n- url: https://www.silentpush.com/trust/\n\
  \  http_status: 404\n  fetched: '2026-08-27'\n- url: https://www.silentpush.com/security/\n  http_status: 404\n  fetched: '2026-08-27'\n- url: https://www.silentpush.com/terms-of-use/\n  http_status: 200\n  fetched: '2026-08-27'\n  finding: no certification keyword present\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silent-push/refs/heads/main/security/silent-push-trust-center.yml
summary_line: trust center published
tags:
- Company
- Security
- Threat Intelligence
- Cybersecurity
- DNS
- Domain Intelligence
- Passive DNS
- Enrichment
- Threat Feeds
- WHOIS
- Model Context Protocol
trust_url: ''
---
