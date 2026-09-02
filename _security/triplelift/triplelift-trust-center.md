---
certifications: []
description: 'TripleLift operates a Trust Center at trust.triplelift.com. It is a single-page JavaScript application on the Responsive (formerly RFPIO) platform: the served HTML is 4KB, its entire body text is "Please enable JavaScript to continue using this application", and no certification, framework, subprocessor list or policy document appears in any machine-readable response. The Trust Center exists; its contents are not readable by a machine.'
kind: trust-center
layout: security
name: Triplelift Trust Center
name_suffix: Trust Center
overview: TripleLift maintains a public trust center covering its security and compliance posture.
provider_name: TripleLift
provider_slug: triplelift
slug: triplelift-trust-center
source_filename: triplelift-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "name: TripleLift Trust Center\ndescription: >-\n  TripleLift operates a Trust Center at trust.triplelift.com. It is a single-page\n  JavaScript application on the Responsive (formerly RFPIO) platform: the served\n  HTML is 4KB, its entire body text is \"Please enable JavaScript to continue using\n  this application\", and no certification, framework, subprocessor list or policy\n  document appears in any machine-readable response. The Trust Center exists; its\n  contents are not readable by a machine.\ngenerated: '2026-08-12'\nmethod: probed\nsource: https://trust.triplelift.com/\ntrust_center:\n  url: https://trust.triplelift.com/\n  http_status: 200\n  title: Trust Center\n  platform: Responsive (RFPIO) Trust Center — profile-guest bundle\n  machine_readable: false\n  content_bytes_served: 4119\n  rendered_text: 'Trust Center Please enable JavaScript to continue using this application.'\ncertifications: []\ncertifications_note: >-\n  NONE READABLE. No SOC 2, ISO 27001, ISO\
  \ 27017, PCI DSS, HIPAA, FedRAMP, TISAX or\n  CSA STAR claim appears in the Trust Center HTML, on triplelift.com, or in any\n  probed response. This records that nothing could be read — not that TripleLift\n  holds no certifications. Because no certification could be verified, no\n  Compliance pointer is emitted for this provider.\nframeworks_referenced_elsewhere:\n  - name: IAB Europe TCF (GDPR)\n    where: user-sync and OpenRTB Regs documentation\n    note: A privacy/consent framework, not a security certification.\n  - name: IAB CCPA Compliance Framework (us_privacy)\n    where: user-sync documentation\n  - name: IAB Global Privacy Platform (GPP)\n    where: user-sync documentation\nrelated_pages:\n  - url: https://triplelift.com/privacy/\n    http_status: 200\n    type: privacy policy\n  - url: https://triplelift.com/privacy-policy/\n    http_status: 200\n    type: privacy policy (alternate path)\n  - url: https://triplelift.com/security/\n    http_status: 404\n  - url: https://triplelift.com/trust/\n\
  \    http_status: 404\n  - url: https://triplelift.com/legal/\n    http_status: 404\n  - url: https://triplelift.com/terms/\n    http_status: 404\ngaps:\n  - >-\n    A Trust Center whose contents require a JavaScript runtime cannot be read by a\n    procurement bot, a security-questionnaire agent, or any automated vendor-risk\n    process — which is the audience a Trust Center exists to serve. The platform\n    supports guest access; the barrier here is rendering, not authorization.\n  - >-\n    No /.well-known/security.txt is served on any TripleLift host, so there is no\n    machine-discoverable security contact or disclosure policy pointing at the\n    Trust Center either.\nx-evidence:\n  - url: https://trust.triplelift.com/\n    http_status: 200\n    fetched: '2026-08-12'\n  - url: https://triplelift.com/security/\n    http_status: 404\n    fetched: '2026-08-12'\n  - url: https://triplelift.com/.well-known/security.txt\n    http_status: 404\n    fetched: '2026-08-12'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/triplelift/refs/heads/main/security/triplelift-trust-center.yml
summary_line: trust center published
tags:
- Programmatic Advertising
- Native Advertising
- Ad Exchange
- OpenRTB
- Header Bidding
- Connected TV
- Supply Side Platform
- Demand-Side Platform
- GraphQL
- AdTech
- Publisher Reporting
- Real-Time Bidding
trust_url: ''
---
