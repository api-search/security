---
api_specs:
- filename: tealium-auth-api-openapi.yml
  format: yaml
  label: Tealium Auth API
  slug: tealium-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-auth-api-openapi.yml
- filename: tealium-collect-api-openapi.yml
  format: yaml
  label: Tealium Collect API
  slug: tealium-collect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-collect-api-openapi.yml
- filename: tealium-customer-api-openapi.yml
  format: yaml
  label: Tealium Customer API
  slug: tealium-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-customer-api-openapi.yml
- filename: tealium-personalization-api-openapi.yml
  format: yaml
  label: Tealium Personalization API
  slug: tealium-personalization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-personalization-api-openapi.yml
- filename: tealium-privacy-api-openapi.yml
  format: yaml
  label: Tealium Privacy API
  slug: tealium-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-privacy-api-openapi.yml
- filename: tealium-ai-read-openapi.yml
  format: yaml
  label: Tealium AI Read API
  slug: tealium-ai-read-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-ai-read-openapi.yml
certifications:
- SSAE18 SOC 2 Type II
- ISO/IEC 27001
- ISO/IEC 27018
- ISO/IEC 27701:2019
- HIPAA & HITECH
- TISAX
- TX-RAMP
- Cloud Security Alliance (CSA)
- GDPR
- CCPA
description: ''
kind: trust-center
layout: security
name: Tealium Trust Center
name_suffix: Trust Center
overview: Tealium maintains a public trust center documenting SSAE18 SOC 2 Type II, ISO/IEC 27001, ISO/IEC 27018, ISO/IEC 27701:2019, HIPAA & HITECH, TISAX, TX-RAMP, Cloud Security Alliance (CSA), GDPR, and CCPA compliance.
provider_name: Tealium
provider_slug: tealium
slug: tealium-trust-center
source_filename: tealium-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nsource: https://trust.tealium.com/, https://tealium.com/security/\nurl: https://trust.tealium.com/\ncompliance_page: https://tealium.com/security/\ncertifications:\n- SSAE18 SOC 2 Type II\n- ISO/IEC 27001\n- ISO/IEC 27018\n- ISO/IEC 27701:2019\n- HIPAA & HITECH\n- TISAX\n- TX-RAMP\n- Cloud Security Alliance (CSA)\n- GDPR\n- CCPA\nevidence:\n- source: https://trust.tealium.com/\n  keywords:\n  - soc 2\n  - iso 27001\n  - hipaa\n  - trust center\n  - gdpr\n- source: https://tealium.com/security/\n  http_status: 200\n  certifications_named:\n  - HIPAA & HITECH\n  - ISO/IEC 27001\n  - ISO/IEC 27701:2019\n  - ISO/IEC 27018\n  - SSAE18 SOC2 Type II\n  - TISAX\n  - TX-RAMP\n  - Cloud Security Alliance (CSA)\n  note: >-\n    The public Security & Compliance page names four certifications the trust center capture\n    missed — ISO/IEC 27701:2019 (privacy information management), TISAX (automotive sector\n    assessment), TX-RAMP\
  \ (Texas state cloud authorization) and CSA membership. Added here on the\n    2026-08-13 pass.\n\nvulnerability_disclosure:\n  program: false\n  policy_url: null\n  security_contact: null\n  bug_bounty: false\n  security_txt: false\n  probed:\n    - url: https://tealium.com/security/\n      status: 200\n      finding: >-\n        Names certifications but publishes no disclosure policy, no security contact address and no\n        reporting instructions. The only related sentence is \"Tealium strives to keep ahead of\n        attackers by working with security researchers, industry experts, and our customers\" —\n        an assertion of intent with no channel attached.\n    - url: https://tealium.com/vulnerability-disclosure/\n      status: 404\n    - url: https://tealium.com/responsible-disclosure/\n      status: 404\n    - url: https://hackerone.com/tealium\n      status: 404\n    - url: https://bugcrowd.com/tealium\n      status: 404\n    - url: https://tealium.com/.well-known/security.txt\n\
  \      status: 404\n    - url: https://docs.tealium.com/.well-known/security.txt\n      status: 404\n    - url: https://platform.tealiumapis.com/.well-known/security.txt\n      status: 404\n  finding: >-\n    NO published vulnerability disclosure route. A researcher who finds a flaw in Tealium has no\n    documented address to send it to — no security.txt, no policy page, no bug bounty platform\n    listing. This is the clearest single remediation available to Tealium: an RFC 9116\n    /.well-known/security.txt naming a contact would close it in an afternoon. Because there is no\n    program, no VulnerabilityDisclosure artifact and no `Security` pointer are emitted.\n\nx-evidence:\n  checked: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/security/tealium-trust-center.yml
summary_line: SSAE18 SOC 2 Type II, ISO/IEC 27001, ISO/IEC 27018, ISO/IEC 27701:2019, HIPAA & HITECH, TISAX, TX-RAMP, Cloud Security Alliance (CSA), GDPR, CCPA
tags:
- Customer Data Platform
- CDP
- Tag Management
- AudienceStream
- Real-Time Events
- Visitor Profiles
- Audience Segmentation
- Data Collection
- Privacy Compliance
- Personalization
trust_url: https://trust.tealium.com/
---
