---
certification_count: 3
certifications:
- Common Criteria (CC)
- Cryptographic module validation (CMVP / FIPS)
- SOC 3
description: Apple publishes a standing Platform Certifications guide rather than a vendor-style trust portal with a document request form. It names the certification programmes Apple holds across hardware, operating systems and internet services — including Apple Pay, the paid surface reachable from Safari — and is public with no sign-in.
kind: trust-center
layout: security
name: Apple Safari Trust Center
name_suffix: Trust Center
overview: Apple Safari maintains a public trust center documenting Common Criteria (CC), Cryptographic module validation (CMVP / FIPS), and SOC 3 compliance.
provider_name: Apple Safari
provider_slug: apple-safari
slug: apple-safari-trust-center
source_filename: apple-safari-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://support.apple.com/guide/certifications/welcome/web\nspecification: API Commons Trust Center\nspecificationVersion: '0.1'\nprovider: Apple Safari\nproviderId: apple-safari\ndescription: >-\n  Apple publishes a standing Platform Certifications guide rather than a vendor-style\n  trust portal with a document request form. It names the certification programmes Apple\n  holds across hardware, operating systems and internet services — including Apple Pay,\n  the paid surface reachable from Safari — and is public with no sign-in.\ntrust_center:\n  url: https://support.apple.com/guide/certifications/welcome/web\n  name: Apple Platform Certifications\n  gated: false\n  probed:\n    - url: https://support.apple.com/guide/certifications/welcome/web\n      status: 200\n      checked: '2026-09-07'\ncertifications:\n  - name: Common Criteria (CC)\n    scope: Apple hardware, operating systems and services\n    evidence: https://support.apple.com/guide/certifications/welcome/web\n\
  \    detail: Apple publishes Common Criteria certification status information.\n  - name: Cryptographic module validation (CMVP / FIPS)\n    scope: Apple cryptographic modules\n    evidence: https://support.apple.com/guide/certifications/welcome/web\n    detail: Apple publishes cryptographic module validation status information.\n  - name: SOC 3\n    scope: Apple Private Cloud Compute\n    evidence: https://support.apple.com/guide/certifications/welcome/web\n    detail: Apple publishes Private Cloud Compute SOC 3 audit reports.\ncoverage_areas:\n  - Hardware security — Secure Enclave Processor and Apple T2 Security Chip\n  - Operating systems — iOS, iPadOS, macOS, tvOS, visionOS, watchOS\n  - Services — Apple internet services and Apple Pay\n  - National regulations security certifications\n  - Security Compliance Projects for macOS, iOS, iPadOS and visionOS\nstatement: >-\n  \"The certifications cover security controls used in the data center environment and\n  controls that are part\
  \ of the security life cycle\" for Apple services.\nrelated:\n  security_policy: https://webkit.org/security-policy/\n  bounty: https://security.apple.com/bounty/guidelines/\n  security_txt: well-known/apple-safari-security.txt\n  vulnerability_disclosure: security/apple-safari-vulnerability-disclosure.yml\nnote: >-\n  ISO 27001/27017/27018 and SOC 2 were NOT found named on the pages probed for this\n  record and are deliberately not asserted here. Only the programmes Apple names on the\n  certifications guide are listed.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n    url: https://apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apple-safari/refs/heads/main/security/apple-safari-trust-center.yml
summary_line: Common Criteria (CC), Cryptographic module validation (CMVP / FIPS), SOC 3
tags:
- Apple
- Browser
- Privacy
- Web Browser
- Webkit
trust_url: ''
---
